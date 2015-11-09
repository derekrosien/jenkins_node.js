# jenkins_node.js
R&amp;D for Jenkins build server

Repository to test Jenkins CI/CD server for a Node.js project

Tutorial:
http://code.tutsplus.com/tutorials/setting-up-continuous-integration-continuous-deployment-with-jenkins--cms-21511

Additional Changes:

1. Had to add the 'scripts' object to the package.json file
  "scripts": {
    "test": "node_modules/.bin/mocha test/test.js"
  }

