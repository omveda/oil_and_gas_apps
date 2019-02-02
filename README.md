# Sample apps based on mapd-charting

#### Get the mapd-charting source code:
```bash
git clone https://github.com/omnisci/mapd-charting.git
```

#### Install Dependencies:
```bash
cd mapd-charting
yarn install
```

#### Test sample code
The sample code creates a multi-layered pointmap/linemap with time and bar chart using US natural gas and pipeline information. These tables are referred to as 
gas_production_us_2018 - Table with US Natural Gas production information
NaturalGas_Pipelines_US_201804 - US Natural Gas Pipeline information
Once you have the tables setup in your OmniSci cloud or on-premise instance, change the user/password fields in MapdCon().
You can then either modify index.html to call i2enabled_natgas_pipelines.html or simply copy i2enabled_natgas_pipelines.html over index.html. Start the server by typing:
```bash
yarn run start
```

Open browser to http://localhost:8080.

# Synopsis

MapD-Charting is a superfast charting library that works natively with [crossfilter](https://github.com/square/crossfilter) that is based off [dc.js](https://github.com/dc-js/dc.js).  It is designed to work with MapD-Connector and MapD-Crossfilter to create charts instantly with our MapD-Core SQL Database.  Please see [examples](https://github.com/omnisci/mapd-charting/tree/master/example) for further understanding to quickly create interactive charts.
