 * Remote: `mongodump --uri=<DB_URI> --archive=<db_name>.gzip --gzip`
 * LocalDB: `mongodump --db=<db_ame> --archive=<db_name>.gzip --gzip`
 * `mongorestore --db=<db_ame> --archive=<file_locations> --gzip`
 ### If you've authentication
 * `mongorestore  -u USERNAME -p PASSWORD --authenticationDatabase admin --db=<db_ame> --archive=<file_locations> --gzip`
 ### If you want to drop collections before restore [This will not drop collections that are not in dump/backup]
  * `mongorestore --db=<db_ame> --archive=<file_locations> --gzip --drop`
