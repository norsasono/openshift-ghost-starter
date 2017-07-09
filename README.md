# Inside This Package

- Nodejs v.6.9.5 (Recomended from Ghost)
- Ghost 0.11.10 (Latest stabel version)

# How To?

1. Make a new Application using [Node.js 0.10](https://openshift.redhat.com/app/console/application_type/cart!nodejs-0.10)
2. Use this repository as a source.
3. Activate mysql cartridge.
4. Done.

---

Don't worry, I actually used Node v.6.9.5 as the default cartridge because the default Node.js version from Openshift-Ghost-Quickstart is 0.10.** and no longger suppported for the recent Ghost version.

---

Or if you want to use PostgreSQL as your database, you have to edit some lines on `config.js`

Default (mysql)
```
database: {
                client: 'mysql',
                connection: {
                    host     : process.env.OPENSHIFT_MYSQL_DB_HOST,
                    port     : process.env.OPENSHIFT_MYSQL_DB_PORT,
                    user     : process.env.OPENSHIFT_MYSQL_DB_USERNAME,
                    password : process.env.OPENSHIFT_MYSQL_DB_PASSWORD,
                    database : process.env.OPENSHIFT_APP_NAME,
                    charset  : 'utf8'
                },
```

Postgre (postgresql)
```
database: {
                client: 'pg',
                connection: {
                    host     : process.env.OPENSHIFT_POSTGRESQL_DB_HOST,
                    port     : process.env.OPENSHIFT_POSTGRESQL_DB_PORT,
                    user     : process.env.OPENSHIFT_POSTGRESQL_DB_USERNAME,
                    password : process.env.OPENSHIFT_POSTGRESQL_DB_PASSWORD,
                    database : process.env.OPENSHIFT_APP_NAME,
                    charset  : 'utf8'
                },
```

---

# Is it possible to be used to deploy Ghost v 1.0.-Beta in the future?
Possiblly yes, but I haven'tried.

Cheers .. 
