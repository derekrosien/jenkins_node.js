# jenkins_node.js
R&amp;D for Jenkins build server

Repository to test Jenkins CI/CD server for a Node.js project


TUTORIAL:
http://code.tutsplus.com/tutorials/setting-up-continuous-integration-continuous-deployment-with-jenkins--cms-21511


TUTORIAL NOTES:
- GitHub > Webhooks > Jenkins (GitHub Plugin) > Jenkins hook url:
   http://jenkins.bluerush.ca:8080/github-webhook/



TUTORIAL CHANGES:

1. Had to add the 'scripts' object to the package.json file
  "scripts": {
    "test": "node_modules/.bin/mocha test/test.js"
  }

2. Within Jenkins project, within the 'build' section...
  Execute shell (replaced './script/test' with 'npm test'):
    npm install
    npm test
