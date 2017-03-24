Node.js
=======
* [Node for Java Developers](https://node.university/blog/502765/node-for-java-devs)
* [npmjs.com](https://www.npmjs.com/)
* [install | npm Documentation](https://docs.npmjs.com/cli/install)
* [Overview of Blocking vs Non-Blocking | Node.js](https://nodejs.org/en/docs/guides/blocking-vs-non-blocking/)
* [package.json | npm Documentation](https://docs.npmjs.com/files/package.json)
* [Debugging - Getting Started | Node.js](https://nodejs.org/en/docs/guides/debugging_getting_started/)
* [docker-node/BestPractices.md · nodejs/docker-node](https://github.com/nodejs/docker-node/blob/master/docs/BestPractices.md)

More topics in the [Getting Started Guide](https://nodejs.org/en/docs/guides/debugging_getting_started/)
----------------------------------------
* Overview of Blocking vs Non-Blocking
* Debugging - Getting Started
* Anatomy of an HTTP Transaction
* Domain Module Postmortem
* The Node.js Event Loop, Timers, and process.nextTick()
* Dockerizing a Node.js web app
* Easy profiling for Node.js Applications
* Timers in Node.js
* Working with Different Filesystems

jsdoc
-----
* [jsdoc](https://www.npmjs.com/package/jsdoc)
* [Use JSDoc: Getting Started with JSDoc 3](http://usejsdoc.org/about-getting-started.html)
* [swagger-jsdoc](https://www.npmjs.com/package/swagger-jsdoc)
* [docstrap/docstrap - GitHub](https://github.com/docstrap/docstrap)

```bash
./node_modules/.bin/jsdoc test.js -d docs
```

DocStrap also introduces a new documentation tag which can appear inside any example block in source code, or in any fenced code block in markdown: {@lang languageName}, where language can be any of the languages supported by [Sunlight](http://sunlightjs.com/).

When in a doclet, add the tag just after the @example tag like this:

```
@example {@lang xml} <div>This is the most interesting web site ever</div>
```

gulp
----
* [gulp - npm](https://www.npmjs.com/package/gulp)
* [gulp/README.md · gulpjs/gulp](https://github.com/gulpjs/gulp/blob/master/docs/README.md)

```bash
npm install gulp-cli -g
npm install gulp -D
touch gulpfile.js
gulp --help
```

Express
-------
* http://localhost:3000/
* [Express - Node.js web application framework](http://expressjs.com/)
* [Express - npm](https://www.npmjs.com/package/express)
* [Express FAQ](http://expressjs.com/en/starter/faq.html)
* [Frameworks built on Express](http://expressjs.com/en/resources/frameworks.html)

```bash
express --view=pug myapp
cd myapp && npm install
DEBUG=myapp:* npm start
```

Feathers
--------
* [Feathers | Instant Realtime and REST APIs with Node.js](http://feathersjs.com/)
* [Built with Feathers · Feathers Showcase](https://docs.feathersjs.com/why/showcase.html)
* [Virtual Hosting, HTTPS and sub-apps](https://docs.feathersjs.com/middleware/mounting.html)

```bash
npm install -g feathers-cli
mkdir my-app && cd my-app
feathers generate
npm start
```

Almost every app needs authentication so Feathers comes with support for email/password, OAuth and Token (JWT) authentication out of the box.

Instead using the generator, you can build from scratch:

```bash
npm install feathers feathers-hooks feathers-socketio feathers-rest feathers-errors feathers-memory feathers-authentication body-parser
```

feathers-swagger
----------------
* [feathersjs/feathers-swagger](https://github.com/feathersjs/feathers-swagger)

```bash
npm install feathers-swagger --save
npm install feathers feathers-rest feathers-memory feathers-swagger body-parser
```


Yeoman
------
* [yo - npm](https://www.npmjs.com/package/yo)
* [Generators | Yeoman](http://yeoman.io/generators/)
* [yeoman-generator](https://www.npmjs.com/package/yeoman-generator)

```bash
mkdir yo-webapp && cd yo-webapp

# install yo
npm install --global yo bower

# install a generator
npm install --global generator-webapp

# run it
yo webapp

# I'm all done. Running npm install && bower install for you to install the required dependencies. If this fails, try running the command yourself.

```

bower - npm
-----------
* [bower - npm](https://www.npmjs.com/package/bower)

NeDB
----
* [NeDB · The FeathersJS Book](https://docs.feathersjs.com/databases/nedb.html)
* [NeDB basics | 10 minutes guide of NeDB essentials](http://10minbasics.com/nedb-basics/)
* [NeDB: A Lightweight JavaScript Database](http://stackabuse.com/nedb-a-lightweight-javascript-database/)

About the `npm --save` option
-----------------------------
By default, NPM simply installs a package under `node_modules`. When you're trying to install dependencies for your app/module, you would need to first install them, and then add them (along with the appropriate version number) to the `dependencies` section of your package.json.

The `--save` option instructs NPM to include the package inside of the `dependencies` section of your `package.json` automatically, thus saving you an additional step.

In addition, there are the complementary options `--save-dev` and `--save-optional` which save the package under `devDependencies` and `optionalDependencies`, respectively. This is useful when installing development-only packages, like grunt or your testing library.

It's documented in the [documentation](https://docs.npmjs.com/cli/install) for `npm install`
