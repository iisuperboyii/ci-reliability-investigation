1st task
in ci.yml file, line 33, run command is wrong, fixed the run command and pushing again. test-ci was missing in package.json, so changed it to npm test

2nd task
in app.test.js, the timestamp was trying to be given an exact value, this causes errors due to latency. changed the code to match using a pattern. exact matching fails under processor latency in the runner. fixed it by verifying timestamp validity and using regex match

3rd task
in ci.yml file, the permission is too permissive, therefore reducing the contents to read only using the code.
