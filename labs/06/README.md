# Data Cleaning

## Contacts

after reading the csv file, i could answer the all qestions with the following expressions.

### Extract all email addresses from the text.
df = pd.DataFrame(csv_contacts)
df["email"]

### Extract all phone numbers from the text.
df["phone"]

### Extract all names that start with the letter ‘J’.
df.loc[df["name"].str.match(r"^J"), "name"]

### Extract all street names that contain the word 'St'.
df.loc[df["address"].str.match(r".*St.*")]

### Extract the last names of all people.
df["name"].str.extract(r"\s+(\S+)")

### Extract all email domains (part after the @ sign).
df["email"].str.extract(r"@(\S+)")

### Find all entries where the phone number ends with ‘7’.
df[df["phone"].str.endswith(r"7")]

### Extract all instances of first names that end with the letter 'e'.
df["vorname"] = df["name"].str.extract(r"(\S+)\s+")
df[df["vorname"].str.endswith(r"e")]

## Orders

### Extract all order numbers, product codes, prices, and order dates.
def order_numbers():
    orders = pd.read_csv(csv_path_orders)
    print("oreder Numbers: \n",orders["order_number"], "Product Codes \n", orders["product_code"], "Prices \n", orders["price"], "Order Dates \n", orders["order_date"])

if __name__ == "__main__":
    order_numbers()

### Find all orders for products priced over $500.
orders = pd.read_csv(csv_path_orders)
orders["price"] = orders["price"].str.extract(r"\$(\d+\.\d+)").astype(float)
orders[orders["price"] > 500]

### Change the date format to DD/MM/YYYY. (Note the re.sub() method)
import re
pattern = r"(\d+)/(\d+)/(\d+)"
replace_rule = r"\2/\1/\3"
orders["order_date"] = orders["order_date"].apply(lambda x : re.sub(pattern, replace_rule, x))
orders

### Find all orders with the highest number of ordered items.
sorted_orders = orders.sort_values(by="number_of_items", ascending=False)
sorted_orders

### Find the cheapest order(s). (You may want to use Python's min() method.)
cheapest = orders[orders["price"] == orders["price"].min()]
cheapest