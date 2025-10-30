# Disclimer: Hier geht es um Daten, die von Personen als Sensible betrachtet werden können. 

# Open Data

<details>
<summary>Daten Quellen</summary>

    Selbstmord Daten -> https://www.destatis.de/EN/Themes/Society-Environment/Health/Causes-Death/Tables/deaths-suicide-months.html

    DWD - SonnenTage -> https://opendata.dwd.de/climate_environment/CDC/observations_germany/climate/monthly/more_precip/historical/monatswerte_RR_00046_20060101_20241231_hist.zip
</details>
<details>
<summary>Description of the data sets</summary>
    - [deaths-suicide-months](https://www.destatis.de/EN/Themes/Society-Environment/Health/Causes-Death/Tables/deaths-suicide-months.html)
    - [monatswerte_RR_00046_20060101_20241231](https://opendata.dwd.de/climate_environment/CDC/observations_germany/climate/monthly/more_precip/historical/monatswerte_RR_00046_20060101_20241231_hist.zip)
    - monatswerte_RR_00046_20060101_20241231 -> CSV (17x397) & deaths-suicide-months -> HTML Table (13x12)
    - Basic statistics;
    +------+--------+--------+---------+---------+---------+
    | Jahr |  Min   |  Max   | Mittel  | Median  | Range   |
    +------+--------+--------+---------+---------+---------+
    | 2012 |  744   |  932   |  829.2  |  826.0  |  188    |
    | 2013 |  720   |  969   |  847.2  |  846.5  |  249    |
    | 2014 |  762   |  931   |  853.3  |  856.0  |  169    |
    | 2015 |  719   |  933   |  847.3  |  847.0  |  214    |
    | 2016 |  722   |  877   |  824.0  |  852.0  |  155    |
    | 2017 |  682   |  860   |  768.7  |  764.5  |  178    |
    | 2018 |  633   |  867   |  781.3  |  789.5  |  234    |
    | 2019 |  660   |  808   |  749.2  |  767.5  |  148    |
    | 2020 |  664   |  842   |  767.1  |  772.5  |  178    |
    | 2021 |  657   |  848   |  767.1  |  776.0  |  191    |
    | 2022 |  702   |  932   |  853.9  |  844.5  |  230    |
    | 2023 |  766   |  960   |  864.5  |  871.5  |  194    |
    +------+--------+--------+---------+---------+---------+

    - Geographic or temporal coverage; deaths-suicide-months (Germany, 2012-2023) & monatswerte_RR_00046_20060101_20241231_hist (Germany, 2006-2024)
    - License;

        deaths-suicide-months:

        Data licence Germany – attribution – version 2.0 (Datenlizenz Deutschland – Namensnennung – Version 2.0)
        © Statistisches Bundesamt (Destatis), 2025
        BESONDERHEIT; Name nennung ist erforderlich
        LIZENZ: Data licence Germany – attribution – version 2.0

        monatswerte_RR_00046_20060101_20241231:
        Source: Deutscher Wetterdienst (DWD), licensed under Creative Commons Attribution 4.0 International (CC BY 4.0)
        https://creativecommons.org/licenses/by/4.0/

        BESONDERHEIT: "Requires separate permission if not DWD-owned"
        LIZENZ: Creative Commons Attribution 4.0 International (CC BY 4.0)

    4. FAIR Princibles

    +--------------+---------------------------------------------------------------+-------------------------------------------------------------+
    | Principle    | Destatis – Suicide Statistics (2012–2023)                     | DWD – Weather & Climate Data (CC BY 4.0)                    |
    +--------------+---------------------------------------------------------------+-------------------------------------------------------------+
    | Findable     |  Yes – Available via GENESIS-Online database with             |   Yes – Listed on DWD Open Data portal and govdata.de,      |
    |              | searchable metadata (title, time, region, units).             | includes detailed spatial/temporal metadata.                |
    +--------------+---------------------------------------------------------------+-------------------------------------------------------------+
    | Accessible   |  Yes – Freely downloadable without login in CSV/XLSX          |   Yes – Open access via HTTPS and APIs, no registration     |
    |              | formats from official Destatis site.                          | needed; all datasets publicly available.                    |
    +--------------+---------------------------------------------------------------+-------------------------------------------------------------+
    | Interoperable|  Partial – Machine-readable (CSV, XLSX, JSON) but metadata    |   Yes – Standard formats (NetCDF, CSV, JSON) and            |
    |              | not fully compliant with DCAT or ISO 19115 standards.         | INSPIRE/OGC-compliant metadata for geodata.                 |
    +--------------+---------------------------------------------------------------+-------------------------------------------------------------+
    | Reusable     |  Yes – Licensed under Data Licence Germany – BY 2.0;          |  Y es – Licensed under Creative Commons Attribution 4.0;    |
    |              | reuse incl. commercial use allowed with attribution.          | clear reuse rules and citation guidance provided.           |
    +--------------+---------------------------------------------------------------+-------------------------------------------------------------+
    | Overall FAIR |  Strong FAIR compliance, only minor metadata limitations.     |  Fu lly FAIR compliant; exemplary open data implementation. |
    +--------------+---------------------------------------------------------------+-------------------------------------------------------------+
    


</details>