# CDN Router
A CDN routing system based on Geo-IP by DNS

## Setup
Create the locations database :
```
sqlite3 databases/locations.dat < locations.sql
```

Configure your datacenters by creating the file `datacenters.json` :
```
nano datacenters.json
```

> Datacenters.json example:
> ```
> {
>   "us": "<us server ip>",
>   "fr": "<france server ip>",
>   "cn": "<china server ip>"
> }
> ```

The database structure should be :
```
router.js
/databases
  |- locations.dat
  |- coordinates.json
  |- datacenters.json
```
