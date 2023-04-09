# python-web-flask-api-csv-to-elasticsearch-client-sqlalchemy-raw-sql-pop

## Description
Reads a csv file into a single node for data in `pop-demo` document.

Uses sqlalchemy to connect and executes raw sql.

Remotely tested with *testify*.

## Tech stack
- python
    - flask
    - sqlalchemy
    - elasticsearch
    - elasticsearch_dbapi
    - testify
    - requests
- elasticsearch
- kibana

## Docker stack
- python
- elasticsearch
- kibana

## To run
`sudo ./install.sh -u`
- Get all pops: http://localhost/pop
  - Schema id, name, and color
- CRUD opperations
  - Read: http://localhost/pop/<id>
  - Unsupported
    - Create: curl -i -X PUT localhost/pop/<id>
    - Update: curl -i -X POST localhost/pop/<id>/<name>/<color>
    - Delete: curl -i -X DELETE localhost/pop/<id>

## To stop (optional)
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`
