# bcrypt-promise
<<<<<<< HEAD

promisify node bcrypt library

### usage:

```bash
    npm install bcrypt-promisfy
```

### example with koa
```javascript
    // require library and initiate koa server
    let bcrypt = require('bcrypt-promise');
    let koa = require('koa');
    let app = koa();
    app.listen(3000);

    // use bcrypt
    app.use(function*(next){
        // get password from somewhere
        let password = this.request.body.password;
        // get hash from somewhere
        let hash = yield db.findHash(_id);

        // **use this library**
        let same = yield bcrypt.compare(password, hash);
        if(same) {
            this.body = 'Yeah';
        } eles {
            this.body = 'Whops';
        }
        yield next;
    });
```
=======
promisify bcrypt library
>>>>>>> 22b91a1f49c61baf0cd8545e2260848671016a10
