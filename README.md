# mocha-rp-agent

Agent for integration Mocha with ReportPortal.
[ReportPortal](http://reportportal.io/)<br>
[ReportPortal on GitHub](https://github.com/reportportal)

### How to use
1. Install the agent in your project:
```cmd
npm i mocha-reportportal-agent --save-dev
```
2. Add reporter to mocha options:
```javascript
require('./mocha-reportportal-reporter.js');

    mochaOpts: {
        colors: true,
        reporter: 'mocha-reportportal-reporter',
        reporterOptions: {
            // client settings
            token: "00000000-0000-0000-0000-000000000000",
            endpoint: "http://your-instance.com:8080/api/v1",
            launch: "LAUNCH_NAME",
            project: "PROJECT_NAME",
            // agent settings
            attachPicturesToLogs: true,
            showPassedHooks: false
        },
        timeout: 600000
    },



### Settings
Agent settings consist of two parts:
* Client settings can be viewed [here](https://github.com/reportportal/client-javascript#settings)
* Agent settings are described below

Parameter | Description
--------- | -----------
attachPicturesToLogs | It is 'true' or 'false', if set 'true' then attempts will be made to attach screenshots to the logs. Default: 'true'.

# Copyright Notice
Licensed under the [GPLv3](https://www.gnu.org/licenses/quick-guide-gplv3.html)
license (see the LICENSE.txt file).

		