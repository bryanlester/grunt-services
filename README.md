# grunt-services

> Start and Stop database services

## Getting Started
This plugin requires Grunt.

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-services --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-services');
```

## The Tasks

All tasks are plain tasks, which means you have to include them in `grunt.registerTask()` statements or call them directly from command line. The available tasks are:

* **startRedis** Start Redis database.
* **startMongo** Start Mongodb database.
* **startPostgres** Start Postgres database.
* **stopRedis** Stop Redis database.
* **stopMongo** Stop Mongodb database.
* **stopPostgres** Stop Postgres database.


### Sample Setup

Create `start` and `stop` aliases for starting and stoping the services:

```js

grunt.initConfig({ /* ... */ });

grunt.registerTask('start', 'Start all required services', ['startRedis', 'startMongo']);
grunt.registerTask('stop', 'Stop all services', ['stopRedis', 'stopMongo']);
```

## Release History
- **v0.0.1**, *15 Feb 2014*
    - Big Bang

## License
Copyright (c) 2014 Thanasis Polychronakis. Licensed under the MIT license.
