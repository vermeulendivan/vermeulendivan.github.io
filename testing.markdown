---
layout: page
title: Testing
permalink: /testing/
---

# Testing plugin
The plugin or changes to the plugin can be tested using Github Actions (https://github.com/kartoza/stream_feature_extractor/actions).
Tests will be performed on each of the methods (e.g. feature extraction) by comparing the result to existing data in the ‘/test’ folder. The following QGIS versions are tested:
1. 3.10;
2. 3.12;
3. 3.14;
4. 3.16 LTR;
5. 3.18;
6. 3.20;
7. 3.22; and
8. latest version.

## Local testing
To perform local testing the 'run-docker-tests.sh' can be used. The shell script can be used as follows:
1. Open your terminal/console;
2. Go to the root directory of the plugin;
3. Type "./run-docker-test.sh" and press enter;
4. The result should be as follows:

![segment_center](/images/testing/local_testing.png)

5. If there is any errors the user will need to investigate.

## Github actions
Tests can manually be performed, but the action should execute automatically. Here is the steps for manual execution:
1. On the repository click on the Actions tab, and select the ‘Test’ worksflow (will execute .github/workflows/test.yml);
2. Click on the Run workflow drop-down and select the Branch you want to perform the test on;
3. Click Run workflow;

![actions](/images/testing/github_actions.png)

4. Processing might take a while, especially if the docker images needs to be pulled;
5. If processing is done, check if the one of the jobs succeeded or failed.

Failed:

![failed](/images/testing/failed.png)

Success:

![success](/images/testing/success.png)

### Failed
If the testing failed, the user needs to investigate the cause of the error. Here is a quick guide on how to do this:
1. Select the test which failed;
2. Select the job which failed (e.g. ‘test (release-3_16)’);
3. The user will be presented with the job steps. Select the job which failed (e.g. ‘Run test suite’);

![success](/images/testing/job_steps.png)

4. A list of print lines will be shown, with the error at the end; and

![error](/images/testing/error_msg.png)

5. Investigate the code to which the error relates to the method performed during that test. Having a look at the data used for the test may also be useful.

### Success
There should be no issue if the tests does not fail. The jobs will be similar to the following:

![jobs_success](/images/testing/jobs_success.png)

The plugin and any updates to the plugin should work with no issue for each of the QGIS versions in the above list.
