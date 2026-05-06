# NoSQL-MongoDB-Testing

This repository contains NoSQL testing and query examples using MongoDB with migrated <strong><a href="https://github.com/xzilla/pagila">Pagila</a></strong> dataset.

Since Pagila is a relational database, it was *migrated* to **MongoDB** to simulate NoSQL data validation scenarios.

> <strong>Data Migration Process:</strong>
<ol>
    <li>Export data from PostgreSQL (CSV format)</li>
    <li>Import data into MongoDB using mongoimport</li>
</ol>

<strong>Example:</strong>
1. For each table: `COPY store TO 'path/store.csv' CSV HEADER;`;
2. Import CSV into the database via PowerShell in the folder with csv files (`path/`): `mongoimport --uri="your_uri" --collection=store --type=csv --headerline --file="store.csv"`.

> <strong>Included Files:</strong>
<ul>
    <li><strong><a href="https://drive.google.com/file/d/1kzOvvsq3eTbMMAevooLJaEB7TniScanO/view?usp=sharing">15 mongo queries</a></strong></li>
    Contains 15 MongoDB queries:
    <ul>
        <li>Find()</li>
        <li>Aggregation pipelines</li>
        <li>Filtering and projections</li>
    </ul>
    <li><strong><a href="https://drive.google.com/drive/folders/1kQQvf3de1yZHDYip6g4_DAVNb1i2zV6M?usp=sharing">Query Results (JSON)</strong></a>. Each query has a corresponding result file (e.g. mongo_query_01_first_10_customers.json)</li>
</ul>
