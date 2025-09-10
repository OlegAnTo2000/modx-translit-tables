## Install

### Download and install translit extra

Install modx/translit extra

### Download table(s)

go to modx project root

```bash
cd /to/modx/root/
```

go to modx core translit tables directory

```bash
cd core/components/translit/model/modx/translit/tables/
```

download table (change <TABLENAME> to real name)
```
wget https://raw.githubusercontent.com/OlegAnTo2000/modx-translit-tables/refs/heads/main/<TABLENAME>.php
```

windows
```bash
iwr https://raw.githubusercontent.com/OlegAnTo2000/modx-translit-tables/refs/heads/main/<TABLENAME>.php -OutFile <TABLENAME>.php
```

get all
```
wget https://raw.githubusercontent.com/OlegAnTo2000/modx-translit-tables/refs/heads/main/czech.php
wget https://raw.githubusercontent.com/OlegAnTo2000/modx-translit-tables/refs/heads/main/kazakh.php
wget https://raw.githubusercontent.com/OlegAnTo2000/modx-translit-tables/refs/heads/main/polish.php
wget https://raw.githubusercontent.com/OlegAnTo2000/modx-translit-tables/refs/heads/main/ukrainian.php
```

### Set tablename in MODx system settings (or context settings)

in MODx settings (or set different tables for different contexts use CrossContextsSettings)
```
friendly_alias_translit = tablename
friendly_alias_translit_class = modx.translit.modTransliterate
friendly_alias_translit_class_path = {core_path}components/translit/model/
```

