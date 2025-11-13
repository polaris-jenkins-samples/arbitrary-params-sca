# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Arbitrary_Sca_Scan/main`
- **Build Number:** #2
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 2 min 43 sec and counting
- **Timestamp:** 2025-11-13 13:05:25 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 0a25c06dd41988e342c3ed7378dc4e5932f5e5e0
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/_Polaris_Arbitrary_Sca_Scan_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Fetching without tags
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
 > git rev-list --no-walk e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/polaris-jenkins-samples/arbitrary-params-sca.git
 > git init /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2 # timeout=10
Fetching upstream changes from https://github.com/polaris-jenkins-samples/arbitrary-params-sca.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/polaris-jenkins-samples/arbitrary-params-sca.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Avoid second fetch
Checking out Revision 0a25c06dd41988e342c3ed7378dc4e5932f5e5e0 (main)
Commit message: "Passing Detect tools from Polaris Scans"
First time build. Skipping changelog.
 > git config remote.origin.url https://github.com/polaris-jenkins-samples/arbitrary-params-sca.git # timeout=10
 > git config --add remote.origin.fetch +refs/heads/main:refs/remotes/origin/main # timeout=10
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 0a25c06dd41988e342c3ed7378dc4e5932f5e5e0 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Polaris_Arbitrary_Sca_Scan/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm
[Pipeline] {
[Pipeline] sh
+ node --version
v22.16.0
[Pipeline] sh
+ npm --version
10.9.2
[Pipeline] sh
+ npm install
npm warn deprecated fsevents@1.2.9: fsevents 1 will break on node v14+ and could be using insecure binaries. Upgrade to fsevents 2.
npm warn deprecated set-value@2.0.0: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated mixin-deep@1.3.1: Critical bug fixed in v2.0.1, please upgrade to the latest version.
npm warn deprecated ini@1.3.5: Please update to ini >=1.3.6 to avoid a prototype pollution issue
npm warn deprecated set-value@0.4.3: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated path-is-absolute@2.0.0: This package is no longer relevant as Node.js 0.12 is unmaintained.
npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
npm warn deprecated har-validator@5.1.3: this library is no longer supported
npm warn deprecated to-iso-string@0.0.2: to-iso-string has been deprecated, use @segment/to-iso-string instead.
npm warn deprecated cryptiles@2.0.5: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
npm warn deprecated bcrypt-nodejs@0.0.3: bcrypt-nodejs is no longer actively maintained. Please use bcrypt or bcryptjs. See https://github.com/kelektiv/node.bcrypt.js/wiki/bcrypt-vs-brypt.js to learn more about these two options
npm warn deprecated cryptiles@0.2.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated source-map-url@0.4.0: See https://github.com/lydell/source-map-url#deprecated
npm warn deprecated boom@0.4.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated boom@2.10.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated chokidar@2.1.6: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@0.2.4: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
npm warn deprecated chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@1.0.9: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated querystring@0.2.0: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
npm warn deprecated request@2.36.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated tough-cookie@2.2.2: ReDoS vulnerability parsing Set-Cookie https://nodesecurity.io/advisories/130
npm warn deprecated hoek@0.9.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm warn deprecated source-map-resolve@0.5.2: See https://github.com/lydell/source-map-resolve#deprecated
npm warn deprecated har-validator@2.0.6: this library is no longer supported
npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated hoek@2.16.3: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated request@2.79.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.88.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.67.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated readdir-scoped-modules@1.0.2: This functionality has been moved to @npmcli/fs
npm warn deprecated hawk@1.0.0: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated hawk@3.1.3: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated jade@0.26.3: Jade has been renamed to pug, please install the latest version of pug instead of jade
npm warn deprecated swig@1.4.2: This package is no longer maintained
npm warn deprecated bson@1.0.9: Fixed a critical issue with BSON serialization documented in CVE-2019-2391, see https://bit.ly/2KcpXdo for more details
npm warn deprecated nodeunit@0.9.5: you are strongly encouraged to use other testing options

added 962 packages, and audited 1412 packages in 13s

32 packages are looking for funding
  run `npm fund` for details

137 vulnerabilities (9 low, 35 moderate, 57 high, 36 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues possible (including breaking changes), run:
  npm audit fix --force

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (polaris-arbitrary-sast)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Arbitrary_Sca_Scan
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [POLARIS]
[Security Scan] INFO: Parameters for polaris:
[Security Scan] INFO:  --- polaris_waitForScan = true
[Security Scan] INFO:  --- polaris_server_url = https://poc.polaris.blackduck.com
[Security Scan] INFO:  --- polaris_assessment_types = SAST,SCA
[Security Scan] INFO:  --- polaris_access_token = ******************************************************************************
[Security Scan] INFO:  --- detect_search_depth = 3
[Security Scan] INFO:  --- detect_args = --detect.diagnostic=true
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Polaris parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Arbitrary_Sca_Scan
[Security Scan] INFO: Polaris Application Name: arbitrary-params-sca
[Security Scan] INFO: Polaris Project Name: arbitrary-params-sca
[Security Scan] INFO: Polaris Branch Name: main
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Arbitrary_Sca_Scan
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/polaris_input16373385195976687054.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 13:03:12.7040 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 13:03:12.7131 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 13:03:14.0743 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 13:03:14.0743 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 13:03:14.0743 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 13:03:14.0743 IST [Bridge CLI] INFO: detect.args = --detect.diagnostic=true [polaris_input16373385195976687054.json]
2025-11-13 13:03:14.0744 IST [Bridge CLI] INFO: detect.search.depth = 3 [polaris_input16373385195976687054.json]
2025-11-13 13:03:14.0744 IST [Bridge CLI] INFO: network.airgap = false [polaris_input16373385195976687054.json]
2025-11-13 13:03:14.0744 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input16373385195976687054.json]
2025-11-13 13:03:14.0744 IST [Bridge CLI] INFO: polaris.application.name = arbitrary-params-sca [polaris_input16373385195976687054.json]
2025-11-13 13:03:14.0744 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input16373385195976687054.json]
2025-11-13 13:03:14.0744 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input16373385195976687054.json]
2025-11-13 13:03:14.0744 IST [Bridge CLI] INFO: polaris.project.name = arbitrary-params-sca [polaris_input16373385195976687054.json]
2025-11-13 13:03:14.0744 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input16373385195976687054.json]
2025-11-13 13:03:14.0744 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input16373385195976687054.json]
2025-11-13 13:03:14.0745 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 13:03:14.0745 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 13:03:14.0764 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 13:03:14.0764 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 13:03:14.0764 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 13:03:14.0764 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 13:03:14.1532 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 13:03:14.1568 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 13:03:14.1570 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 13:03:14.1570 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 13:03:14.1601 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 13:03:14.1603 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 13:03:14.1603 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 13:03:16.8149 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "061CJMT"
2025-11-13 13:03:16.8153 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "GUZNL1T"
2025-11-13 13:03:16.8371 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 13:03:16.8375 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 13:03:16.8378 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 13:03:16.8382 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 13:03:16.8387 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 13:03:16.8390 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 13:03:16.8393 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 13:03:16.8396 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 13:03:16.8421 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 13:03:16.8424 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 13:03:16.8436 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 13:03:16.8564 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 13:03:16.9033 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 13:03:16.9085 IST [Check pull request] INFO: Adapter finished
2025-11-13 13:03:16.9744 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 13:03:16.9750 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 13:03:17.7336 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 13:03:17.7336 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 13:03:17.7344 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 13:03:17.8388 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 13:03:18.1222 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 13:03:18.1223 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 13:03:18.4536 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 13:03:18.4540 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 13:03:18.4541 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 13:03:18.5507 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 13:03:18.8449 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 13:03:18.8450 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 13:03:18.8450 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 13:03:19.1486 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 13:03:19.1487 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 13:03:19.2264 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 13:03:19.2291 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 13:03:19.5187 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 13:03:19.5421 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 13:03:19.5423 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 13:03:19.5429 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 13:03:19.5430 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 13:03:19.5430 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 13:03:19.5430 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 13:03:19.5430 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 13:03:19.5460 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 13:03:19.5460 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 13:03:19.5460 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 13:03:19.5460 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 13:03:19.5460 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 13:03:19.5460 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 13:03:19.5500 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 13:03:19.5815 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 13:03:19.5820 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 13:03:19.5821 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 13:03:19.5933 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 13:03:19.5935 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 13:03:19.5935 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 13:03:19.6487 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 13:03:19.6495 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect
2025-11-13 13:03:19.7114 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 13:03:19.7114 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache3471275559/.authKey
2025-11-13 13:03:19.7115 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=58c35df8-0a5c-4a85-811e-7821367e7737
2025-11-13 13:03:19.7115 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 13:03:19.7115 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 13:03:19.7115 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 13:03:19.7136 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 13:03:19.7136 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 13:03:19.7150 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir create
2025-11-13 13:03:19.7805 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 13:03:19.7808 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 13:03:20.6355 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 13:03:20.6370 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 13:03:21.1639 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 13:03:21.1792 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 13:03:21.6916 IST [Polaris Coverity Capture] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir'
2025-11-13 13:03:21.6918 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 13:03:21.9995 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 13:03:22.2615 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 13:03:22.5409 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 13:03:22.8111 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 13:03:23.0783 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 13:03:23.3483 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 13:03:23.6327 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 13:03:23.9171 IST [Polaris Coverity Capture] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 13:03:23.9172 IST [Polaris Coverity Capture] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 13:03:23.9172 IST [Polaris Coverity Capture] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 13:03:23.9227 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 13:03:24.1890 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 13:03:24.4591 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 13:03:24.7255 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 13:03:25.1056 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 13:03:25.3767 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 13:03:25.3957 IST [Polaris Coverity Capture] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 13:03:25.3957 IST [Polaris Coverity Capture] INFO:           and it will not be updated.
2025-11-13 13:03:25.8819 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 13:03:26.3483 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 13:03:26.9326 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-1853961 --record-with-source
2025-11-13 13:03:26.9611 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 13:03:26.9751 IST [Polaris Coverity Capture] INFO: Emitting 84 Files.
2025-11-13 13:03:27.4872 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 13:03:27.4902 IST [Polaris Coverity Capture] INFO: Executing action No unwanted TUs to delete
2025-11-13 13:03:27.4903 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 13:03:27.4904 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 13:03:27.4906 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 13:03:27.5124 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 13:03:27.5125 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-444612815/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 13:03:27.5524 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 13:03:27.5524 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 13:03:27.5524 IST [Polaris Coverity Capture] INFO: 
2025-11-13 13:03:29.2449 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 13:03:29.8054 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 13:03:29.8623 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 13:03:29.8623 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 87
2025-11-13 13:03:29.8623 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 13:03:29.8625 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 13:03:29.8625 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 13:03:29.8625 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 87
2025-11-13 13:03:29.8625 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32921
2025-11-13 13:03:29.8648 IST [Polaris Coverity Capture] INFO: Capture phase took 9.232s.
2025-11-13 13:03:29.8649 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 13:03:29.8649 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 13:03:29.8649 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 13:03:29.8649 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 13:03:29.8649 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 13:03:29.8908 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 13:03:29.8928 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 13:03:29.8998 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 13:03:29.8999 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 13:03:29.9001 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 13:03:29.9003 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 13:03:29.9024 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 13:03:29.9025 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 13:03:29.9026 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 13:03:29.9622 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.detector.search.depth=3 --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true --detect.diagnostic=true
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 13:03:30.7548 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 13:03:30.7549 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 13:03:30.7549 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 13:03:30.7549 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 13:03:30.7549 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 13:03:30.7549 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 13:03:30.7549 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:03:30.8836 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:03:30.8837 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 13:03:30.8837 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.detector.search.depth = 3 [cmd] 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.diagnostic = true [cmd] 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge [env] 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845
2025-11-13 13:03:30.9716 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:03:30.9716 IST [Polaris SCA Package Manager Scan] INFO: ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
2025-11-13 13:03:30.9716 IST [Polaris SCA Package Manager Scan] INFO: Diagnostic mode on.
2025-11-13 13:03:30.9717 IST [Polaris SCA Package Manager Scan] INFO: A zip file will be created with logs and relevant Detect output files.
2025-11-13 13:03:30.9717 IST [Polaris SCA Package Manager Scan] INFO: It is generally not recommended to leave diagnostic mode on as you must manually clean up the zip.
2025-11-13 13:03:30.9717 IST [Polaris SCA Package Manager Scan] INFO: ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
2025-11-13 13:03:30.9718 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Initializing diagnostic components.
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/reports/search_report.txt
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/reports/search_detailed_report.txt
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/reports/detector_report.txt
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/reports/detector_profile_report.txt
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/reports/code_location_report.txt
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/reports/dependency_counts_report.txt
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/reports/detect_configuration.txt
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to capture sysout.
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Writing sysout to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/logs/sysout.txt
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to set 'com.blackduck.integration' logging level.
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to capture additional log messages to files.
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Redirected to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/logs/all.txt
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Redirected to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/logs/debug.txt
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Redirected to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/logs/info.txt
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to restrict console to debug level (additional levels written to files).
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Adding additional log listeners to extractions.
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics is now in control of logging!
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating configuration diagnostics reports.
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics system is ready.
2025-11-13 13:03:30.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm (depth 0)
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/package-lock.json
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/package.json
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Saved file to diagnostics zip: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/package-lock.json
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Saved file to diagnostics zip: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/package.json
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 13:03:31.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 13:03:33.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/scan/components-with-locations.json
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/status/status.json
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing diagnostic mode.
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing reports.
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing logging.
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing executable capture.
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing file capture.
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating diagnostics zip.
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics zip location: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/detect-run-2025-11-13-07-33-30-845.zip
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics file created at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/detect-run-2025-11-13-07-33-30-845.zip
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostic mode has completed.
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-33-30-845/scan/components-with-locations.json
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:04:15.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 00m 45s 632ms
2025-11-13 13:04:15.9396 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 13:04:15.9397 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 13:04:15.9399 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 13:04:15.9975 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "fa3250f7-cfa4-4052-a2ba-f769060d6597"
2025-11-13 13:04:15.9979 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "121f045b-5209-4a6b-a32c-8b72b8c21e45"
2025-11-13 13:04:17.5717 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 13:04:17.5918 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 13:04:18.2508 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   7%  16384/207979
2025-11-13 13:04:18.2560 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   4%  16384/386398
2025-11-13 13:04:18.4612 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  39%  81920/207979
2025-11-13 13:04:18.4645 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  70%  147456/207979
2025-11-13 13:04:18.4670 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  29%  114688/386398
2025-11-13 13:04:18.8938 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  207979/207979
2025-11-13 13:04:18.8944 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  55%  212992/386398
2025-11-13 13:04:18.9072 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  80%  311296/386398
2025-11-13 13:04:19.1070 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  386398/386398
2025-11-13 13:04:19.3960 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 13:04:19.6317 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 13:04:19.8586 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "fa3250f7-cfa4-4052-a2ba-f769060d6597"
2025-11-13 13:04:20.1301 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "121f045b-5209-4a6b-a32c-8b72b8c21e45"
2025-11-13 13:04:20.1626 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 13:04:20.1631 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 13:04:20.1639 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 13:04:20.2181 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "121f045b-5209-4a6b-a32c-8b72b8c21e45"
2025-11-13 13:04:20.2185 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "fa3250f7-cfa4-4052-a2ba-f769060d6597"
2025-11-13 13:04:20.9812 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "fa3250f7-cfa4-4052-a2ba-f769060d6597" is "Waiting for Capture"
2025-11-13 13:04:20.9858 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "121f045b-5209-4a6b-a32c-8b72b8c21e45" is "Waiting for Capture"
2025-11-13 13:04:31.2782 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "121f045b-5209-4a6b-a32c-8b72b8c21e45" is "Queuing"
2025-11-13 13:04:31.2875 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "fa3250f7-cfa4-4052-a2ba-f769060d6597" is "Queuing"
2025-11-13 13:05:02.1582 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "121f045b-5209-4a6b-a32c-8b72b8c21e45" is "Scanning"
2025-11-13 13:05:02.2239 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "fa3250f7-cfa4-4052-a2ba-f769060d6597" is "Scanning & Publishing"
2025-11-13 13:05:22.7771 IST [Polaris Waiter] INFO: test with assessment type "SAST(sastFull)" and id "121f045b-5209-4a6b-a32c-8b72b8c21e45" completed successfully
2025-11-13 13:05:22.8430 IST [Polaris Waiter] INFO: test with assessment type "SCA(scaPackage)" and id "fa3250f7-cfa4-4052-a2ba-f769060d6597" completed successfully
2025-11-13 13:05:22.8775 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.completed'
2025-11-13 13:05:22.8778 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.completed'
2025-11-13 13:05:22.8783 IST [Polaris Waiter] INFO: Adapter finished
2025-11-13 13:05:22.9491 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SAST(sastFull)" assessment...
2025-11-13 13:05:22.9497 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SCA(scaPackage)" assessment...
2025-11-13 13:05:23.7536 IST [Polaris Policy Checker] INFO: no policies were violated to break the build
2025-11-13 13:05:23.7751 IST [Polaris Policy Checker] INFO: Adapter finished
2025-11-13 13:05:23.8118 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SAST(sastFull)" assessment
2025-11-13 13:05:23.8124 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SCA(scaPackage)" assessment
2025-11-13 13:05:24.5769 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SAST(sastFull)" with id "121f045b-5209-4a6b-a32c-8b72b8c21e45"
 {
 "critical": 0,
 "high": 2,
 "informational": 0,
 "low": 25,
 "medium": 13
}
2025-11-13 13:05:24.5873 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SCA(scaPackage)" with id "fa3250f7-cfa4-4052-a2ba-f769060d6597"
 {
 "critical": 6,
 "high": 109,
 "informational": 0,
 "low": 15,
 "medium": 133
}
2025-11-13 13:05:24.6117 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.low'
2025-11-13 13:05:24.6118 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.high'
2025-11-13 13:05:24.6120 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.informational'
2025-11-13 13:05:24.6121 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.critical'
2025-11-13 13:05:24.6123 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.medium'
2025-11-13 13:05:24.6124 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.low'
2025-11-13 13:05:24.6126 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.medium'
2025-11-13 13:05:24.6127 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.critical'
2025-11-13 13:05:24.6129 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.high'
2025-11-13 13:05:24.6131 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.informational'
2025-11-13 13:05:24.6134 IST [Polaris Issues Fetcher] INFO: Adapter finished
2025-11-13 13:05:24.6546 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "fa3250f7-cfa4-4052-a2ba-f769060d6597" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/c74085a9-3515-4731-b208-47bf96fcc3d9/projects/9963ef92-dad4-4c25-a4f3-ecdf53758bd2/tests/fa3250f7-cfa4-4052-a2ba-f769060d6597/detected-issues
2025-11-13 13:05:24.6551 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "121f045b-5209-4a6b-a32c-8b72b8c21e45" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/c74085a9-3515-4731-b208-47bf96fcc3d9/projects/9963ef92-dad4-4c25-a4f3-ecdf53758bd2/tests/121f045b-5209-4a6b-a32c-8b72b8c21e45/detected-issues
2025-11-13 13:05:24.6551 IST [Polaris Status Provider] INFO: Polaris issues view for project "arbitrary-params-sca", branch "main" is available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/c74085a9-3515-4731-b208-47bf96fcc3d9/projects/9963ef92-dad4-4c25-a4f3-ecdf53758bd2/issues?branchId=06b81732-20fc-462b-bf07-21fe21e314fe
2025-11-13 13:05:24.6651 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 13:05:24.6653 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 13:05:24.6655 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 13:05:24.6658 IST [Polaris Status Provider] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 303
[Security Scan] INFO: Security Scan execution is successful
**************************** END EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
Black Duck Logs Publisher - Starting log upload process
[Pipeline] echo
Configuration: [githubOrg:polaris-jenkins-samples, repoName:arbitrary-params-sca, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_Polaris_Arbitrary_Sca_Scan/main
[Pipeline] echo
Build Number: 2
[Pipeline] echo
GitHub Organization: polaris-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: arbitrary-params-sca
[Pipeline] echo
Target repository: polaris-jenkins-samples/arbitrary-params-sca
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*