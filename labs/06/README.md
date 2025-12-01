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