# Sample apps based on mapd-charting

#### Get the mapd-charting source code:
```git clone https://github.com/omnisci/mapd-charting.git
```

#### Install Dependencies:
```cd mapd-charting
yarn install
```

#### Test sample code
The sample code creates a multi-layered pointmap/linemap with time and bar chart using US natural gas and pipeline information. These tables are referred to as 
gas_production_us_2018 - Table with US Natural Gas production information
NaturalGas_Pipelines_US_201804 - US Natural Gas Pipeline information
Once you have the tables setup in your OmniSci cloud or on-premise instance, change the user/password fields in MapdCon().
You can then either modify index.html to call i2enabled_natgas_pipelines.html or simply copy i2enabled_natgas_pipelines.html over index.html. Start the server by typing:
```yarn run start
```

Open browser to http://localhost:8080.
Dimensional charting built to work natively with crossfilter rendered using d3.js.


# Synopsis

MapD-Charting is a superfast charting library that works natively with [crossfilter](https://github.com/square/crossfilter) that is based off [dc.js](https://github.com/dc-js/dc.js).  It is designed to work with MapD-Connector and MapD-Crossfilter to create charts instantly with our MapD-Core SQL Database.  Please see [examples](#examples) for further understanding to quickly create interactive charts.

Our [Tweetmap Demo](https://www.mapd.com/demos/tweetmap/) was made only using MapD-Charting.

# Documentation

Visit our [API Docs](http://mapd.github.io/mapd-charting/docs/) for additional information on MapD Charting

# Testing

New components in MapD-Charting should be unit-tested and linted.  All tests will be in the same folder as the new component.

```
+-- src
|   +-- /mixins/new-mixin-component.js
|   +-- /mixins/new-mixin-component.unit.spec.js
```

The linter and all tests run on
```bash
yarn run test
```

To check only unit-tests run:
```bash
yarn run test:unit
```

### Linting

Please lint all your code in `mapd-charting/`. The lint config file can be found in `.eslintrc.json`.  For new components, please fix all lint warnings and errors.

# Scripts

| Command        | Description  |
--- | ---
`yarn run start` | Copies files for examples and then serves the example
`yarn run build` | Runs webpack and builds js and css in `/dist`
`yarn run docs` | Creates and opens docs
`yarn run test` | Runs both linting and unit tests
`yarn run clean` | Removes node modules, dist, docs, and example files

# Documentation
The charting library uses [documentation.js](https://github.com/documentationjs/documentation) for API documentation. Docs can be built and viewed locally with the `npm run docs` command.

## Contributing

Interested in contributing? We'd love for you to help! Check out [Contributing.MD](.github/CONTRIBUTING.md)
