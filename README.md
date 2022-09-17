# Total.js QueryBuilder: TotalDB

A simple QueryBuilder integrator for Total DB.

- [Documentation](https://docs.totaljs.com/total4/)
- `$ npm install querybuildertotaldb`

__Initialization__:

```js
// require('querybuilderdb').init(name, url, [errorhandling]);
// name {String} a name of DB (default: "default")
// url {String} a URL address to the Total DB instance
// errorhandling {Function(err, cmd)}

require('querybuildertotaldb').init('default', CONF.database);
```

__Usage__:

```js
DB().find('tbl_user').where('id', 1234).callback(console.log);
// DB('default').find('tbl_user').where('id', 1234).callback(console.log);
```