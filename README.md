# Awesome DuckDB [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) <!-- omit in toc -->

> A curated list of awesome DuckDB libraries, tools and resources.

[DuckDB](https://duckdb.org/) is an in-process SQL OLAP database management system.

<!-- omit in toc -->
## Contents

- [Resources](#resources)
- [Client APIs](#client-apis)
- [Tools Powered by DuckDB](#tools-powered-by-duckdb)
  - [Web Clients](#web-clients)
- [Libraries Powered by DuckDB](#libraries-powered-by-duckdb)
- [SQL Clients and IDE that Support DuckDB](#sql-clients-and-ide-that-support-duckdb)
- [NoSQL Clients and Libraries](#nosql-clients-and-libraries)
- [Projects Powered by DuckDB](#projects-powered-by-duckdb)
- [Integrations](#integrations)
- [Extensions](#extensions)
- [Media](#media)
  - [Talks](#talks)
  - [Podcasts](#podcasts)
  - [Blog Posts](#blog-posts)
- [Contribute](#contribute)

## Resources

- [Official Documentation](https://duckdb.org/docs/) - Official DuckDB documentation.
  - [Official Blog](https://duckdb.org/news/) - Official DuckDB blog.
  - [DuckDB Clients](https://duckdb.org/docs/api/overview) - Client APIs for DuckDB.
  - [DuckDB Documentation PDF](https://duckdb.org/duckdb-docs.pdf) - The DuckDB documentation as a single PDF file.
- [docker-duckdb](https://github.com/davidgasquez/docker-duckdb) - Docker image for DuckDB CLI.
- [DuckDB setup](https://github.com/marketplace/actions/duckdb-setup) - GitHub Action to install DuckDB in CI.
- [Serverless DuckDB over S3](https://github.com/BauplanLabs/quack-reduce/) - Running DuckDB over a data lake on S3 using lambda.
- [DuckDB snippets](https://duckdbsnippets.com/) - Collection of snippets curated by MotherDuck.
- [DuckDB tldr page](https://tldr.inbrowser.app/pages/common/duckdb) - DuckDB's entry in [tldr pages](https://tldr.sh/), available in CLI via the `tldr duckdb` command.
- [DuckDB AWS Lambda layer](https://github.com/tobilg/duckdb-nodejs-layer) - Run DuckDB in AWS Lambda functions.
- [Compatible DuckDB Extensions for AWS Lambda](https://extensions.quacking.cloud/) - Extensions specifically compiled for the AWS Lambda runtime (GLIBC 2.26).
- [Serverless DuckDB as API](https://github.com/tobilg/serverless-duckdb) - Use DuckDB as API with Amazon API Gateway and AWS Lambda.
- [Serverless Parquet Repartitioner](https://github.com/tobilg/serverless-parquet-repartitioner) - Use DuckDB to repartition data in S3-based Data Lakes.
- [Observable notebooks](https://observablehq.com/search?query=duckdb&sort=created&direction=desc&useES=true) - Notebooks using DuckDB on the Observable data visualization platform.
- [duckdb-nf](https://github.com/edmundmiller/duckdb-nf) - Example uses of DuckDB with Nextflow.

## Client APIs

- [C](https://duckdb.org/docs/api/c/overview)
- [C++](https://duckdb.org/docs/api/cpp)
- [CLI](https://duckdb.org/docs/api/cli)
- [Go](https://github.com/marcboeker/go-duckdb)
- [Julia](https://duckdb.org/docs/api/julia)
- [Node.js](https://duckdb.org/docs/api/nodejs/overview)
- [Python](https://duckdb.org/docs/api/python/overview)
- [R](https://duckdb.org/docs/api/r)
- [Rust](https://github.com/duckdb/duckdb-rs)
- [Swift](https://duckdb.org/docs/api/swift)
- [TypeScript](https://www.npmjs.com/package/duckdb-async)
- [Wasm](https://duckdb.org/docs/api/wasm/overview)
- [ADBC](https://duckdb.org/docs/api/adbc)
- [ODBC](https://duckdb.org/docs/api/odbc/overview)
- [.NET](https://github.com/Giorgi/DuckDB.NET/)
- [Common Lisp](https://github.com/ak-coram/cl-duckdb)

## Tools Powered by DuckDB

- [Rill Developer](https://github.com/rilldata/rill-developer) - Tool for effortlessly transforming data sets into powerful, opinionated dashboards using SQL.
- [Ibis Project](https://ibis-project.org/) - A DataFrame API for interacting with DuckDB (and other compute engines).
- [MotherDuck](https://motherduck.com/) - Serverless data warehouse powered by DuckDB.
- [Boiling Data](https://boilingdata.com/) - Serverless data analytics overlay on top of S3 Data Lakes.
- [Hex Dataframe SQL](https://learn.hex.tech/docs/explore-data/cells/sql-cells/sql-cells-introduction) - Hex's Dataframe SQL cells are powered by DuckDB.
- [Mode](https://mode.com/blog/how-we-switched-in-memory-data-engine-to-duck-db-to-boost-visual-data-exploration-speed/) - Mode uses DuckDB for their in-memory data engine.
- [VulcanSQL](https://vulcansql.com/) - DuckDB can be used as a caching layer or a data connector in VulcanSQL, a Data API framework for data folks to create REST APIs by writing SQL templates.
- [Tad](https://www.tadviewer.com) - A fast, free, cross-platform tabular data viewer application powered by DuckDB.
- [Honeycomb Maps](https://docs.honeycomb.place/) - A browser-based geospatial analysis tool leveraging DuckDB Wasm.
- [Bauplan](https://www.bauplanlabs.com/) - A serverless data transformation platform for data lakes.
- [Excalichart.com](http://www.excalichart.com/) - A fast, free dashboard for exploring your data.
- [Malloy](https://www.malloydata.dev/) - Malloy is an experimental language for describing data relationships and transformations. Malloy connects to BigQuery and Postgres, and natively supports DuckDB.
- [Evidence](https://evidence.dev) - Generate reports using SQL and markdown. The DuckDB connector allows querying across DuckDB, csv, parquet and json.
- [Latitude](https://latitude.so) - Latitude uses DuckDB to power data snapshots. Drop a CSV file and query it with SQL at the speed of light.
- [Census](https://www.getcensus.com/) - Census's dataset diffing for incremental syncs is powered by DuckDB.
- [Huey](https://github.com/rpbouman/huey) - Blazing-fast & intuitive pivot tables on .parquet, .csv, .json files and .duckdb tables in the browser based on DuckDB WASM. Open source (MIT). Zero install!
- [Parquet Explorer](https://marketplace.visualstudio.com/items?itemName=AdamViola.parquet-explorer) - Visual Studio Code extension for exploring Parquet files with SQL, powered by DuckDB.
- [Iceburst](https://iceburst.io) - The real-time data lake for monitoring & security.
- [DQOps](https://dqops.com) - Data quality platform for data engineers, data quality teams and data operations.

### Web Clients

- [Online DuckDB Shell](https://shell.duckdb.org/) - Online DuckDB shell powered by WebAssembly.
- [SQL Workbench](https://sql-workbench.com) - DuckDB-WASM based SQL Workbench for running queries on local or remote data, being able to show data as tables or visually as graphs, and sharing queries via URLs.
- [Sekuel Playground](https://sekuel.com/playground/) - Query your local parquet, csv, json. Your data will not be sent out of the device you are using.
- [CSVFiddle](https://csvfiddle.io/) - Free tool to explore and share insights from CSV files using SQL. Import data, write SQL, then instantly share it with anyone.
- [Codapi](https://codapi.org/duckdb/) - Embed executable code snippets directly into your product documentation, online course or blog post.
- [QuackDB](https://app.quackdb.com/) - Open-source online DuckDB SQL playground and editor.

## Libraries Powered by DuckDB

- [Mosaic](https://uwdata.github.io/mosaic/) - An extensible framework for linking databases and interactive views.
- [Fugue](https://github.com/fugue-project/fugue/) - A unified interface for distributed computing. Fugue executes SQL, Python, Pandas, and Polars code on Spark, Dask and Ray without any rewrites.
- [Splink](http://github.com/moj-analytical-services/splink) - A free Python library for fast, accurate data deduplication and record linkage.
- [Simple-data-analysis](https://github.com/nshiab/simple-data-analysis) - Easy-to-use and high-performance JavaScript library for data analysis.
- [duckdb_fdw](https://github.com/alitrack/duckdb_fdw) - DuckDB Foreign Data Wrapper for PostgreSQL.
- [@jetblack/duckdb-react](https://github.com/rob-blackbourn/jetblack-duckdb-react) - A context manager for React and duckdb-wasm.
- [QuackOSM](https://github.com/kraina-ai/quackosm) - A Python library for downloading and transforming raw OpenStreetMap data into GeoParquet files.

## SQL Clients and IDE that Support DuckDB

- [Harlequin](https://harlequin.sh) - The DuckDB IDE for your terminal. ([GitHub](https://github.com/tconbeer/harlequin)).
- [qStudio](https://www.timestored.com/qstudio/) - A free SQL tool specialized for data analysts. It runs on every operating system and allows easy browsing of tables and charting of results.
- [DuckDB SQL Tools](https://marketplace.visualstudio.com/items?itemName=RandomFractalsInc.duckdb-sql-tools) - Free DuckDB SQL Tools for VS Code IDE. [Premium version available](https://github.com/RandomFractals/pro-data-tools/blob/main/duckdb-tools.md#duckdb-pro-tools) with advanced features.
- [VSCode SQLTools (Free)](https://marketplace.visualstudio.com/items?itemName=Evidence.sqltools-duckdb-driver) - Free open-source VSCode extension to query and explore your DuckDB databases with latest DuckDB support.
- [DBeaver](https://dbeaver.com) - DBeaver is a universal database access and development tool that can be used to connect almost any type of database.
- [DataGrip](https://www.jetbrains.com/datagrip/) - Paid SQL IDE by Jetbrains that supports many different database technologies, including DuckDB.
- [Duckling](https://github.com/l1xnan/duckling) - A fast viewer for CSV/Parquet files and DuckDB/SQLite, based on Tauri.

## NoSQL Clients and Libraries

- [nodbi](https://docs.ropensci.org/nodbi/) - NoSQL Database Connector for R, providing a common API across Elasticsearch, CouchDB, MongoDB, SQLite, PostgreSQL, and DuckDB

## Projects Powered by DuckDB

- [NBA Monte Carlo](https://github.com/matsonj/nba-monte-carlo) - Monte Carlo simulation of the NBA season, leveraging Meltano, dbt, DuckDB and Evidence.
- [Datadex](https://github.com/davidgasquez/datadex/) - Open source and local friendly data platform to collaborate on Open Data using DuckDB, Dagster, dbt, and Quarto.
- [`endoflife.date` database](https://www.kaggle.com/datasets/adriensales/endoflife-date-database)

## Integrations

- [dbt-duckdb](https://github.com/jwills/dbt-duckdb) - DuckDB dbt adapter.
- [data load tool - DuckDB destination](https://dlthub.com/docs/dlt-ecosystem/destinations/duckdb) - Extract and load data from APIs to DuckDB using dlt.
- [target-duckdb](https://hub.meltano.com/loaders/target-duckdb/) - Load data to DuckDB based on Singer spec.
- [Airbyte DuckDB destination](https://docs.airbyte.com/integrations/destinations/duckdb/) - Load data to DuckDB with Airbyte.
- [Kestra DuckDB plugin](https://kestra.io/plugins/plugin-jdbc-duckdb) - Run queries with DuckDB to schedule data transformations and process automations, and run event-driven anomaly detection pipelines.
- [Arrow Flight SQL Server](https://github.com/voltrondata/flight-sql-server-example) - An example implementation of the [Arrow Flight SQL protocol](https://arrow.apache.org/docs/format/FlightSql.html) what runs in a client-server setup with DuckDB or SQLite as backends.
- [SQLFlow](https://github.com/turbolytics/sql-flow) - Enables SQL-based stream-processing, powered by DuckDB.
- [nf-sqldb](https://github.com/nextflow-io/nf-sqldb) - This plugin provides support for interacting with SQL databases in Nextflow scripts.

## Extensions

- [Official Extensions](https://duckdb.org/docs/extensions/overview.html) - Official DuckDB extensions.
  - [`arrow`](https://github.com/duckdblabs/arrow) - A zero-copy data integration between Apache Arrow and DuckDB.
  - [`duckdb_iceberg`](https://github.com/duckdblabs/duckdb_iceberg) - For reading Iceberg tables.
  - [`duckdb_aws`](https://github.com/duckdblabs/duckdb_aws) - For handling AWS credentials.
  - [`duckdb_azure`](https://github.com/duckdblabs/duckdb_azure) - For using the Azure Blob storage.
  - [`mysql`](https://duckdb.org/docs/extensions/mysql) - To read from and write to MySQL databases.
  - [`postgres`](https://duckdb.org/docs/extensions/postgres) - To read from and write to PostgreSQL databases.
  - [`spatial`](https://duckdb.org/docs/extensions/spatial) - Enables geospatial processing.
  - [`sqlite`](https://duckdb.org/docs/extensions/sqlite) - To read from and write to SQLite databases.
- [DuckDB Extension Radar](https://github.com/mehd-io/duckdb-extension-radar) - Repository that contains DuckDB extensions on GitHub. Refreshed daily.
- [Deltatable](https://github.com/Mause/duckdb-deltatable-extension) - DuckDB extension for reading Delta tables.
- [Lance](https://github.com/eto-ai/lance/tree/main/integration/duckdb_lance) - Integrate Lance (modern columnar data format for ML implemented in Rust) with DuckDB.
- [PRQL](https://github.com/ywelsch/duckdb-prql) - Run PRQL commands directly within DuckDB.
- [duckdb-engine](https://github.com/Mause/duckdb_engine) - SQLAlchemy driver for DuckDB.
- [Scrooge-McDuck](https://github.com/pdet/Scrooge-McDuck) - DuckDB extension to support a set of aggregation functions and data scanners on financial data.
- [duckdb-pytables](https://github.com/MarkRoddy/duckdb-pytables) - DuckDB extension to allow running SQL on arbitrary data sources.
- [ODBC Scanner DuckDB Extension](https://github.com/rupurt/odbc-scanner-duckdb-extension) - DuckDB extension to read data directly from databases supporting the ODBC interface.
- [duckdb-jfr-extension](https://github.com/ocadaruma/duckdb-jfr-extension) - DuckDB extension to read JFR (Java Flight Recorder) files directly.
- [QDuckDB](https://gitlab.com/Oslandia/qgis/qduckdb) - Plugin for reading DuckDB spatial tables in QGIS software.
- [ERPL](https://erpl.io) - DuckDB SAP connector using RFC, ODP, or BICS.
- [duckdb-extension-template-zig](https://github.com/rupurt/duckdb-extension-template-zig) - A Zig & Nix toolkit template for building extensions against multiple versions of DuckDB using Zig, C or C++.
- [DuckPGQ](https://github.com/cwida/duckpgq-extension) - DuckDB extension for graph workloads that supports the SQL/PGQ standard.

## Media

### Talks

- [DuckCon #4 playlist](https://www.youtube.com/playlist?list=PLzIMXBizEZjhZcTiEFZIAxPpB6RE9TmgC)
– [State of the Duck @ DuckCon #4](https://www.youtube.com/watch?v=cyZfpXxXojE) - Hannes Mühleisen and Mark Raasveldt.
- [In-Process Analytical Data Management with DuckDB @ PyData Amsterdam](https://www.youtube.com/watch?v=5ddoZR6PYNU) - Hannes Mühleisen.
- [DuckDB: The Power of a Data Warehouse in your Python Process @ PyData Yerevan](https://www.youtube.com/watch?v=q_SKaOeRiOI) - Gábor Szárnyas.
- [DuckDB: Bringing analytical SQL directly to your Python shell @ EuroPython](https://www.youtube.com/watch?v=egN4TwVyJss) - Pedro Holanda.
- [DuckDB keynote @ Data + AI Summit 2023](https://www.youtube.com/watch?v=GaHWuQ_cBhA) - Hannes Mühleisen.
- [State of the Duck @ DuckCon #3](https://www.youtube.com/watch?v=LlkEnaOkzdk) - Hannes Mühleisen and Mark Raasveldt.
- [DuckCon #3 playlist](https://www.youtube.com/playlist?list=PLzIMXBizEZjhy6QG4Eqoe9k9NgBa-w67Y)
- [DuckDB: Bringing Analytical SQL Directly To Your Python Shell @ FOSDEM](https://www.youtube.com/watch?v=-rCZQHXSunc) - Pedro Holanda.
- [State of the Duck @ DuckCon #2](https://www.youtube.com/watch?v=rdnPkLSkoyU) - Hannes Mühleisen & Mark Raasveldt.
- [DuckDB Extensions @ DuckCon](https://www.youtube.com/watch?v=UKo_LQyLTko) - Pedro Holanda & Sam Ansmink.
- [Developing Systems in Academia: The Good, the Bad, and the not-so-Ugly Duckling @ CIDR](https://www.youtube.com/watch?v=dv4A2LIFG80) - Hannes Mühleisen.
- [DuckDB An Embeddable Analytical Database @ FOSDEM](https://www.youtube.com/watch?v=nPDomZQ8jI4) - Hannes Mühleisen.
- [DuckDB tutorials playlist by Learn Data with Mark](https://www.youtube.com/watch?v=fZj6kTwXN1U&list=PLw2SS5iImhEThtiGNPiNenOr2tVvLj6H7) - Mark Needham.
- [DuckDB tutorials playlist by MotherDuck](https://www.youtube.com/playlist?list=PLIYcNkSjh-0wlrFUE2VvQilLU2aBPns0K) - Mehdi Ouazza (MotherDuck).
- [Nextflow and database uses: powering data engineering, exploring DuckDB, and beyond](https://youtu.be/GknH1u3NtGI?si=PKnF__cQJ_citMUi) - Edmund Miller.

### Podcasts

- [Developer Voices: Implementing Hardware-Friendly Databases](https://www.youtube.com/watch?v=pZV9FvdKmLc) - Hannes Mühleisen.
- [The Geek Narrator: DuckDB Internals](https://www.youtube.com/watch?v=f9QlkXW4H9A) - Mark Raasveldt.
- [Software Engineering Daily: DuckDB](https://softwareengineeringdaily.com/2022/03/18/duckdb-with-hannes-muleisen/) - Hannes Mühleisen.
- [Data Engineering Podcast: Move Your Database To The Data And Speed Up Your Analytics With DuckDB](https://www.dataengineeringpodcast.com/duckdb-in-process-olap-database-episode-270/) - Hannes Mühleisen.
- [The Analytics Engineering Podcast: The Personal Data Warehouse](https://podtail.com/en/podcast/the-analytics-engineering-podcast/the-personal-data-warehouse-w-jordan-tigani-of-mot/) - Jordan Tigani.

### Blog Posts

- [Modern Data Stack in a Box](https://duckdb.org/2022/10/12/modern-data-stack-in-a-box.html) -  Fast, free, and open-source Modern Data Stack deployed on a laptop using the combination of DuckDB, Meltano, dbt, and Apache Superset.
- [How to use DuckDB, Motherduck and Kestra for ETL](https://motherduck.com/blog/motherduck-kestra-etl-pipelines/) - How DuckDB can transform data, mask sensitive PII information, detect anomalies in event-driven workflows, and streamline reporting use cases.
- [DuckDB vs. MotherDuck — how do they compare](https://kestra.io/blogs/2023-07-28-duckdb-vs-motherduck) - What are key differences between them, and when to choose each of these options.
- [Building DuckDB Extensions with Zig and Nix](https://rupurt.github.io/posts/building-duckdb-extensions-with-zig-and-nix) - For Nix users and Zig developers familiar with DuckDB looking to extend it’s capabilities with custom extensions.
- [Exploring StarCraft 2 data with Airflow, DuckDB and Streamlit](https://medium.com/data-engineer-things/exploring-starcraft-2-data-with-airflow-duckdb-and-streamlit-7c0ad79f9ca6) - Example project using DuckDB to persist API data, but also explains how to use DuckDB as a versatile data manipulation tool in data wrangling scripts.

## Contribute

Contributions welcome! Read the [contribution guidelines](CONTRIBUTING.md) first.
