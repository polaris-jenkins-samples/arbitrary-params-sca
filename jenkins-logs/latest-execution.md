# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Arbitrary_Sca_Scan/main`
- **Build Number:** #3
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 2 min 33 sec and counting
- **Timestamp:** 2025-11-13 13:10:31 UTC

---

## Console Output

```
Started by user admin
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 959e1df5d044d6b3900697edcf7bcbb15e2361b3
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
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Fetching changes from the remote Git repository
Fetching without tags
 > git rev-parse --resolve-git-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/.git # timeout=10
 > git config remote.origin.url https://github.com/polaris-jenkins-samples/arbitrary-params-sca.git # timeout=10
Fetching upstream changes from https://github.com/polaris-jenkins-samples/arbitrary-params-sca.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/polaris-jenkins-samples/arbitrary-params-sca.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Checking out Revision 959e1df5d044d6b3900697edcf7bcbb15e2361b3 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 959e1df5d044d6b3900697edcf7bcbb15e2361b3 # timeout=10
Commit message: "Passing detect tools from Polaris"
 > git rev-list --no-walk 0a25c06dd41988e342c3ed7378dc4e5932f5e5e0 # timeout=10
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
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm
[Pipeline] {
[Pipeline] sh
+ node --version
v22.16.0
[Pipeline] sh
+ npm --version
10.9.2
[Pipeline] sh
+ npm install

up to date, audited 1480 packages in 20s

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
[Pipeline] { (polaris-arbitrary-sca)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm
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
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/polaris_input7900347496813135755.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 13:08:37.8523 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 13:08:37.8597 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 13:08:39.2042 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 13:08:39.2043 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 13:08:39.2043 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 13:08:39.2043 IST [Bridge CLI] INFO: detect.args = --detect.diagnostic=true [polaris_input7900347496813135755.json]
2025-11-13 13:08:39.2043 IST [Bridge CLI] INFO: detect.search.depth = 3 [polaris_input7900347496813135755.json]
2025-11-13 13:08:39.2043 IST [Bridge CLI] INFO: network.airgap = false [polaris_input7900347496813135755.json]
2025-11-13 13:08:39.2043 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input7900347496813135755.json]
2025-11-13 13:08:39.2043 IST [Bridge CLI] INFO: polaris.application.name = arbitrary-params-sca [polaris_input7900347496813135755.json]
2025-11-13 13:08:39.2043 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input7900347496813135755.json]
2025-11-13 13:08:39.2043 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input7900347496813135755.json]
2025-11-13 13:08:39.2043 IST [Bridge CLI] INFO: polaris.project.name = arbitrary-params-sca [polaris_input7900347496813135755.json]
2025-11-13 13:08:39.2043 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input7900347496813135755.json]
2025-11-13 13:08:39.2044 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input7900347496813135755.json]
2025-11-13 13:08:39.2044 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 13:08:39.2044 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 13:08:39.2061 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 13:08:39.2062 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 13:08:39.2062 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 13:08:39.2062 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 13:08:39.2831 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 13:08:39.2863 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 13:08:39.2865 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 13:08:39.2869 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 13:08:39.2900 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 13:08:39.2902 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 13:08:39.2902 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 13:08:41.8144 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "JXA9WCP"
2025-11-13 13:08:41.8155 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "SIAZS43"
2025-11-13 13:08:41.8438 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 13:08:41.8441 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 13:08:41.8443 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 13:08:41.8446 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 13:08:41.8449 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 13:08:41.8458 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 13:08:41.8460 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 13:08:41.8462 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 13:08:41.8464 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 13:08:41.8466 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 13:08:41.8473 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 13:08:41.8671 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 13:08:41.9174 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 13:08:41.9176 IST [Check pull request] INFO: Adapter finished
2025-11-13 13:08:41.9692 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 13:08:41.9697 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 13:08:42.7281 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 13:08:42.7282 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 13:08:42.7288 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 13:08:42.8022 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 13:08:43.0959 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 13:08:43.0960 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 13:08:43.3908 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 13:08:43.3909 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 13:08:43.3910 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 13:08:43.5254 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 13:08:43.8187 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 13:08:43.8189 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 13:08:43.8189 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 13:08:44.1200 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 13:08:44.1201 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 13:08:44.1938 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 13:08:44.1971 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 13:08:44.5001 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 13:08:44.5305 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 13:08:44.5307 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 13:08:44.5310 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 13:08:44.5312 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 13:08:44.5312 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 13:08:44.5312 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 13:08:44.5312 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 13:08:44.5343 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 13:08:44.5344 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 13:08:44.5344 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 13:08:44.5344 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 13:08:44.5344 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 13:08:44.5344 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 13:08:44.5353 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 13:08:44.5689 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 13:08:44.5695 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 13:08:44.5696 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 13:08:44.5785 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 13:08:44.5786 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 13:08:44.5787 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 13:08:44.6478 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 13:08:44.6484 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect
2025-11-13 13:08:44.7053 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 13:08:44.7054 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache3498580094/.authKey
2025-11-13 13:08:44.7054 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=58c35df8-0a5c-4a85-811e-7821367e7737
2025-11-13 13:08:44.7055 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 13:08:44.7055 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 13:08:44.7056 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 13:08:44.7073 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 13:08:44.7073 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 13:08:44.7090 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir create
2025-11-13 13:08:44.7804 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 13:08:44.7808 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 13:08:45.6224 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 13:08:45.6252 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 13:08:46.3259 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 13:08:46.3408 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 13:08:46.8047 IST [Polaris Coverity Capture] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir'
2025-11-13 13:08:46.8048 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 13:08:47.1059 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 13:08:47.3792 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 13:08:47.6525 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 13:08:47.9274 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 13:08:48.1786 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 13:08:48.4323 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 13:08:48.6997 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 13:08:48.9512 IST [Polaris Coverity Capture] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 13:08:48.9512 IST [Polaris Coverity Capture] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 13:08:48.9512 IST [Polaris Coverity Capture] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 13:08:48.9558 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 13:08:49.2194 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 13:08:49.4834 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 13:08:49.7487 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 13:08:50.0048 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 13:08:50.2604 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 13:08:50.2807 IST [Polaris Coverity Capture] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 13:08:50.2807 IST [Polaris Coverity Capture] INFO:           and it will not be updated.
2025-11-13 13:08:50.7723 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 13:08:51.2148 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 13:08:51.7901 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-841805646 --record-with-source
2025-11-13 13:08:51.8173 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 13:08:51.8303 IST [Polaris Coverity Capture] INFO: Emitting 84 Files.
2025-11-13 13:08:52.3285 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 13:08:52.3304 IST [Polaris Coverity Capture] INFO: Executing action No unwanted TUs to delete
2025-11-13 13:08:52.3304 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 13:08:52.3306 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 13:08:52.3309 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 13:08:52.3603 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 13:08:52.3604 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-4244231541/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 13:08:52.4031 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 13:08:52.4031 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 13:08:52.4031 IST [Polaris Coverity Capture] INFO: 
2025-11-13 13:08:54.0811 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 13:08:54.6010 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 13:08:54.6584 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 13:08:54.6584 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 87
2025-11-13 13:08:54.6584 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 13:08:54.6584 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 13:08:54.6584 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 13:08:54.6585 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 87
2025-11-13 13:08:54.6585 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32921
2025-11-13 13:08:54.6607 IST [Polaris Coverity Capture] INFO: Capture phase took 9.041s.
2025-11-13 13:08:54.6608 IST [Polaris Coverity Capture] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 13:08:54.6608 IST [Polaris Coverity Capture] WARNING: 
2025-11-13 13:08:54.6608 IST [Polaris Coverity Capture] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 13:08:54.6608 IST [Polaris Coverity Capture] WARNING:   * C#
2025-11-13 13:08:54.6608 IST [Polaris Coverity Capture] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 13:08:54.6849 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 13:08:54.6869 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 13:08:54.6941 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 13:08:54.6942 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 13:08:54.6944 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 13:08:54.6946 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 13:08:54.6961 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 13:08:54.6962 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 13:08:54.6962 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 13:08:54.7297 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.detector.search.depth=3 --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true --detect.diagnostic=true
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 13:08:55.8040 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 13:08:55.8041 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 13:08:55.8041 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 13:08:55.8042 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 13:08:55.8042 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 13:08:55.8043 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 13:08:55.8044 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:08:55.9345 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:08:55.9345 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 13:08:55.9345 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.detector.search.depth = 3 [cmd] 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.diagnostic = true [cmd] 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge [env] 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:08:55.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897
2025-11-13 13:08:56.0247 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:08:56.0248 IST [Polaris SCA Package Manager Scan] INFO: ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
2025-11-13 13:08:56.0248 IST [Polaris SCA Package Manager Scan] INFO: Diagnostic mode on.
2025-11-13 13:08:56.0248 IST [Polaris SCA Package Manager Scan] INFO: A zip file will be created with logs and relevant Detect output files.
2025-11-13 13:08:56.0248 IST [Polaris SCA Package Manager Scan] INFO: It is generally not recommended to leave diagnostic mode on as you must manually clean up the zip.
2025-11-13 13:08:56.0248 IST [Polaris SCA Package Manager Scan] INFO: ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
2025-11-13 13:08:56.0248 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Initializing diagnostic components.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/reports/search_report.txt
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/reports/search_detailed_report.txt
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/reports/detector_report.txt
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/reports/detector_profile_report.txt
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/reports/code_location_report.txt
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/reports/dependency_counts_report.txt
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Created report file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/reports/detect_configuration.txt
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to capture sysout.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Writing sysout to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/logs/sysout.txt
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to set 'com.blackduck.integration' logging level.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to capture additional log messages to files.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Redirected to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/logs/all.txt
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Redirected to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/logs/debug.txt
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Redirected to file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/logs/info.txt
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Attempting to restrict console to debug level (additional levels written to files).
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Adding additional log listeners to extractions.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics is now in control of logging!
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating configuration diagnostics reports.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics system is ready.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm (depth 0)
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/package-lock.json
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/package.json
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Saved file to diagnostics zip: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/package-lock.json
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Saved file to diagnostics zip: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/package.json
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 13:08:56.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 13:08:58.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/scan/components-with-locations.json
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/status/status.json
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing diagnostic mode.
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing reports.
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing logging.
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing executable capture.
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Finishing file capture.
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating diagnostics zip.
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics zip location: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/detect-run-2025-11-13-07-38-55-897.zip
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostics file created at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/detect-run-2025-11-13-07-38-55-897.zip
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Diagnostic mode has completed.
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-07-38-55-897/scan/components-with-locations.json
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 13:09:42.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 00m 47s 083ms
2025-11-13 13:09:42.1483 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 13:09:42.1485 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 13:09:42.1487 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 13:09:42.1872 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "b384e7ad-0006-4be6-8e8a-4b9103268d64"
2025-11-13 13:09:42.1877 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "4ec25305-e7ce-4843-bcbb-4ae293bf065d"
2025-11-13 13:09:43.5258 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 13:09:43.5536 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 13:09:43.9876 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   4%  16384/385594
2025-11-13 13:09:43.9955 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:   7%  16384/212931
2025-11-13 13:09:44.2002 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  29%  114688/385594
2025-11-13 13:09:44.2145 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  38%  81920/212931
2025-11-13 13:09:44.2147 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  69%  147456/212931
2025-11-13 13:09:44.6342 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  212931/212931
2025-11-13 13:09:44.6508 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  55%  212992/385594
2025-11-13 13:09:44.6547 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  80%  311296/385594
2025-11-13 13:09:44.8724 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  385594/385594
2025-11-13 13:09:45.1635 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 13:09:45.3583 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Polaris_Arbitrary_Sca_Scan_main/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 13:09:45.6388 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "4ec25305-e7ce-4843-bcbb-4ae293bf065d"
2025-11-13 13:09:45.8593 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "b384e7ad-0006-4be6-8e8a-4b9103268d64"
2025-11-13 13:09:45.9027 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 13:09:45.9033 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 13:09:45.9097 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 13:09:45.9818 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "4ec25305-e7ce-4843-bcbb-4ae293bf065d"
2025-11-13 13:09:45.9824 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "b384e7ad-0006-4be6-8e8a-4b9103268d64"
2025-11-13 13:09:46.7621 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "b384e7ad-0006-4be6-8e8a-4b9103268d64" is "Queuing"
2025-11-13 13:09:46.7631 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "4ec25305-e7ce-4843-bcbb-4ae293bf065d" is "Queuing"
2025-11-13 13:09:57.0743 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "4ec25305-e7ce-4843-bcbb-4ae293bf065d" is "Scanning & Publishing"
2025-11-13 13:09:57.0815 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "b384e7ad-0006-4be6-8e8a-4b9103268d64" is "Scanning"
2025-11-13 13:10:28.0329 IST [Polaris Waiter] INFO: test with assessment type "SAST(sastFull)" and id "b384e7ad-0006-4be6-8e8a-4b9103268d64" completed successfully
2025-11-13 13:10:28.0330 IST [Polaris Waiter] INFO: test with assessment type "SCA(scaPackage)" and id "4ec25305-e7ce-4843-bcbb-4ae293bf065d" completed successfully
2025-11-13 13:10:28.0593 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.completed'
2025-11-13 13:10:28.0604 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.completed'
2025-11-13 13:10:28.0611 IST [Polaris Waiter] INFO: Adapter finished
2025-11-13 13:10:28.1361 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SAST(sastFull)" assessment...
2025-11-13 13:10:28.1367 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SCA(scaPackage)" assessment...
2025-11-13 13:10:29.2146 IST [Polaris Policy Checker] INFO: no policies were violated to break the build
2025-11-13 13:10:29.2309 IST [Polaris Policy Checker] INFO: Adapter finished
2025-11-13 13:10:29.2713 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SAST(sastFull)" assessment
2025-11-13 13:10:29.2721 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SCA(scaPackage)" assessment
2025-11-13 13:10:30.0401 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SAST(sastFull)" with id "b384e7ad-0006-4be6-8e8a-4b9103268d64"
 {
 "critical": 0,
 "high": 2,
 "informational": 0,
 "low": 25,
 "medium": 13
}
2025-11-13 13:10:30.0520 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SCA(scaPackage)" with id "4ec25305-e7ce-4843-bcbb-4ae293bf065d"
 {
 "critical": 6,
 "high": 109,
 "informational": 0,
 "low": 15,
 "medium": 133
}
2025-11-13 13:10:30.0790 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.critical'
2025-11-13 13:10:30.0793 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.informational'
2025-11-13 13:10:30.0795 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.low'
2025-11-13 13:10:30.0798 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.medium'
2025-11-13 13:10:30.0800 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.high'
2025-11-13 13:10:30.0803 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.critical'
2025-11-13 13:10:30.0808 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.high'
2025-11-13 13:10:30.0815 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.informational'
2025-11-13 13:10:30.0818 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.low'
2025-11-13 13:10:30.0820 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.medium'
2025-11-13 13:10:30.0828 IST [Polaris Issues Fetcher] INFO: Adapter finished
2025-11-13 13:10:30.1364 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "b384e7ad-0006-4be6-8e8a-4b9103268d64" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/c74085a9-3515-4731-b208-47bf96fcc3d9/projects/9963ef92-dad4-4c25-a4f3-ecdf53758bd2/tests/b384e7ad-0006-4be6-8e8a-4b9103268d64/detected-issues
2025-11-13 13:10:30.1369 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "4ec25305-e7ce-4843-bcbb-4ae293bf065d" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/c74085a9-3515-4731-b208-47bf96fcc3d9/projects/9963ef92-dad4-4c25-a4f3-ecdf53758bd2/tests/4ec25305-e7ce-4843-bcbb-4ae293bf065d/detected-issues
2025-11-13 13:10:30.1369 IST [Polaris Status Provider] INFO: Polaris issues view for project "arbitrary-params-sca", branch "main" is available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/c74085a9-3515-4731-b208-47bf96fcc3d9/projects/9963ef92-dad4-4c25-a4f3-ecdf53758bd2/issues?branchId=06b81732-20fc-462b-bf07-21fe21e314fe
2025-11-13 13:10:30.1460 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 13:10:30.1462 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 13:10:30.1464 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 13:10:30.1466 IST [Polaris Status Provider] INFO: Adapter finished
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
Build Number: 3
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