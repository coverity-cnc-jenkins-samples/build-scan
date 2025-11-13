# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Coverity_Build_Scan/main`
- **Build Number:** #4
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 2 min 34 sec and counting
- **Timestamp:** 2025-11-13 22:09:23 UTC

---

## Console Output

```
Started by user admin
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 407a5c1728bb0665c1fccada94fa704f4db3d3ba
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/_Github_Coverity_Build_Scan_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
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
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Fetching changes from the remote Git repository
Fetching without tags
 > git rev-parse --resolve-git-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/.git # timeout=10
 > git config remote.origin.url https://github.com/coverity-cnc-jenkins-samples/build-scan.git # timeout=10
Fetching upstream changes from https://github.com/coverity-cnc-jenkins-samples/build-scan.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/coverity-cnc-jenkins-samples/build-scan.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Checking out Revision 407a5c1728bb0665c1fccada94fa704f4db3d3ba (main)
Commit message: "Delete jenkins-logs directory"
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 407a5c1728bb0665c1fccada94fa704f4db3d3ba # timeout=10
 > git rev-list --no-walk 1d019fa2c9734ea777774a36ee1ae782a5922302 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Coverity_Build_Scan/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm
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

up to date, audited 1412 packages in 21s

32 packages are looking for funding
  run `npm fund` for details

136 vulnerabilities (9 low, 35 moderate, 57 high, 35 critical)

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
[Pipeline] { (coverity-build-scan)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Build_Scan
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [COVERITY]
[Security Scan] INFO: Parameters for coverity:
[Security Scan] INFO:  --- coverity_passphrase = ******************************************************************************
[Security Scan] INFO:  --- coverity_waitForScan = true
[Security Scan] INFO:  --- coverity_url = https://integrations-qa.dev.cnc.duckutil.net
[Security Scan] INFO:  --- coverity_user = admin
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- network_ssl_trustAll = false
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Coverity parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Build_Scan
[Security Scan] INFO: Coverity Project Name: build-scan
[Security Scan] INFO: Coverity Stream Name: build-scan-main
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Build_Scan
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage connect --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/coverity_input5595390879687386997.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 22:07:27.4012 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 22:07:27.4073 IST [Bridge CLI] INFO: Found version "3.0.128" in registry for workflow "connect", trying to load it from local cache
2025-11-13 22:07:27.4722 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 22:07:27.4722 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 22:07:27.4722 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 22:07:27.4722 IST [Bridge CLI] INFO: coverity.connect.project.name = build-scan [coverity_input5595390879687386997.json]
2025-11-13 22:07:27.4722 IST [Bridge CLI] INFO: coverity.connect.stream.name = build-scan-main [coverity_input5595390879687386997.json]
2025-11-13 22:07:27.4723 IST [Bridge CLI] INFO: coverity.connect.url = https://integrations-qa.dev.cnc.duckutil.net [coverity_input5595390879687386997.json]
2025-11-13 22:07:27.4723 IST [Bridge CLI] INFO: coverity.connect.user.name = admin [coverity_input5595390879687386997.json]
2025-11-13 22:07:27.4723 IST [Bridge CLI] INFO: coverity.connect.user.password = ***************************************** [coverity_input5595390879687386997.json]
2025-11-13 22:07:27.4723 IST [Bridge CLI] INFO: coverity.waitForScan = true [coverity_input5595390879687386997.json]
2025-11-13 22:07:27.4723 IST [Bridge CLI] INFO: network.airgap = false [coverity_input5595390879687386997.json]
2025-11-13 22:07:27.4723 IST [Bridge CLI] INFO: network.ssl.trustAll = false [coverity_input5595390879687386997.json]
2025-11-13 22:07:27.4723 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 22:07:27.4724 IST [Bridge CLI] INFO: Starting adapters for stage connect
2025-11-13 22:07:27.4727 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Controller
2025-11-13 22:07:27.4770 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 22:07:27.5041 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 22:07:27.5043 IST [Check pull request] INFO: Adapter finished
2025-11-13 22:07:30.1298 IST [Coverity Connect Controller] INFO: No coverity version is configured, will use the default or latest supported version from the server
2025-11-13 22:07:30.2124 IST [Coverity Connect Controller] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 22:07:30.2125 IST [Bridge CLI] INFO: Starting adapters for stage connect-post-processing
2025-11-13 22:07:30.2125 IST [Bridge CLI] INFO: Starting adapters for stage scm
2025-11-13 22:07:30.2125 IST [Bridge CLI] INFO: Starting adapters for stage connect-scan
2025-11-13 22:07:30.2129 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Scan
2025-11-13 22:07:30.2129 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Post Scan
2025-11-13 22:07:30.2130 IST [Bridge CLI] INFO: Starting Adapter: SCM Checker
2025-11-13 22:07:30.2133 IST [Coverity Connect Controller] INFO: Adapter finished
2025-11-13 22:07:30.2175 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for Set Version for Coverity
2025-11-13 22:07:30.2176 IST [Default Adapter for Set Version for Coverity] INFO: Provided value for resource 'coverity.version'
2025-11-13 22:07:30.2177 IST [Default Adapter for Set Version for Coverity] INFO: Adapter finished
2025-11-13 22:07:30.2797 IST [Coverity Connect Scan] INFO: Identified workflow: Coverity
2025-11-13 22:07:30.2798 IST [Coverity Connect Scan] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity scan --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -o analyze.location=connect -o commit.connect.url=https://integrations-qa.dev.cnc.duckutil.net -o commit.connect.stream=build-scan-main -o commit.connect.project=build-scan
2025-11-13 22:07:30.3452 IST [Coverity Connect Scan] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 22:07:30.3503 IST [Coverity Connect Scan] WARNING: No setting for 'commit.connect.on-new-cert' specified.
2025-11-13 22:07:30.3504 IST [Coverity Connect Scan] WARNING: Using default value of 'distrust'.
2025-11-13 22:07:30.3504 IST [Coverity Connect Scan] WARNING: This may result in a certificate validation error when uploading defects to Coverity Connect.
2025-11-13 22:07:30.3504 IST [Coverity Connect Scan] WARNING: If you trust the Coverity Connect instance and certificate validation fails, set 'commit.connect.on-new-cert' to 'trust'.
2025-11-13 22:07:30.3504 IST [Coverity Connect Scan] WARNING: If you are unfamiliar with what this means, please talk to your Coverity Connect administrator.
2025-11-13 22:07:30.3538 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir reset-host-name
2025-11-13 22:07:30.4027 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir check-compatible
2025-11-13 22:07:30.4286 IST [Coverity Connect Scan] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 22:07:30.4286 IST [Coverity Connect Scan] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 22:07:32.2880 IST [Coverity Connect Scan] INFO: Cloud analysis is enabled.
2025-11-13 22:07:35.7967 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 22:07:36.6942 IST [Coverity Connect Scan] INFO: Caching is enabled.
2025-11-13 22:07:38.1011 IST [Coverity Connect Scan] INFO: Telemetry is enabled
2025-11-13 22:07:38.7808 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 22:07:38.8071 IST [Coverity Connect Scan] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 22:07:39.2612 IST [Coverity Connect Scan] INFO: Executing action no-op: skipping compiler configuration
2025-11-13 22:07:39.7004 IST [Coverity Connect Scan] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 22:07:40.1278 IST [Coverity Connect Scan] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 22:07:40.6752 IST [Coverity Connect Scan] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/capture-file-list-206444680 --record-with-source
2025-11-13 22:07:40.7008 IST [Coverity Connect Scan] INFO: Buildless capture started.
2025-11-13 22:07:40.7147 IST [Coverity Connect Scan] INFO: Emitting 84 Files.
2025-11-13 22:07:40.9058 IST [Coverity Connect Scan] INFO: Buildless capture completed.
2025-11-13 22:07:40.9074 IST [Coverity Connect Scan] INFO: Executing action No unwanted TUs to delete
2025-11-13 22:07:40.9075 IST [Coverity Connect Scan] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 22:07:40.9076 IST [Coverity Connect Scan] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir
2025-11-13 22:07:40.9078 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 22:07:40.9249 IST [Coverity Connect Scan] INFO: Executing action Invalidate capture results
2025-11-13 22:07:41.4766 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 22:07:41.5324 IST [Coverity Connect Scan] INFO: Capture summary:
2025-11-13 22:07:41.5324 IST [Coverity Connect Scan] INFO:     SUCCEEDED: 84
2025-11-13 22:07:41.5324 IST [Coverity Connect Scan] INFO:     INCOMPLETE: 0
2025-11-13 22:07:41.5324 IST [Coverity Connect Scan] INFO:     FAILED: 0
2025-11-13 22:07:41.5324 IST [Coverity Connect Scan] INFO:     IGNORED: 6
2025-11-13 22:07:41.5324 IST [Coverity Connect Scan] INFO:     FILES CAPTURED: 84
2025-11-13 22:07:41.5325 IST [Coverity Connect Scan] INFO:     LINES OF CODE: 32728
2025-11-13 22:07:41.5349 IST [Coverity Connect Scan] INFO: Capture phase took 3.436s.
2025-11-13 22:07:41.5351 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml'
2025-11-13 22:07:41.5375 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml'
2025-11-13 22:07:41.5387 IST [Coverity Connect Scan] INFO: Analyzing project in the cloud using Coverity Analysis version 2025.9.0
2025-11-13 22:07:41.8406 IST [Coverity Connect Scan] INFO: Creating archive containing data to be analyzed...
2025-11-13 22:07:41.8868 IST [Coverity Connect Scan] INFO: Properties archive created.
2025-11-13 22:07:41.8868 IST [Coverity Connect Scan] INFO: Uploading data for analysis...
2025-11-13 22:07:42.6027 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 22:07:48.3734 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 22:07:48.3735 IST [Coverity Connect Scan] INFO: Scan created.
2025-11-13 22:07:48.3735 IST [Coverity Connect Scan] INFO: The scan ID is 'a89dfc5e-aa45-40c5-9d77-fda9aad95dda'
2025-11-13 22:07:48.3738 IST [Coverity Connect Scan] INFO: Waiting for scan to complete...
2025-11-13 22:07:48.3739 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 22:09:19.4521 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 22:09:20.1546 IST [Coverity Connect Scan] INFO: Analysis summary after merging defects:
2025-11-13 22:09:20.1546 IST [Coverity Connect Scan] INFO:     HIGH SEVERITY:    2 issue(s)
2025-11-13 22:09:20.1547 IST [Coverity Connect Scan] INFO:     MEDIUM SEVERITY: 12 issue(s)
2025-11-13 22:09:20.1547 IST [Coverity Connect Scan] INFO:     LOW SEVERITY:    25 issue(s)
2025-11-13 22:09:20.1547 IST [Coverity Connect Scan] INFO:     AUDIT SEVERITY:   0 issue(s)
2025-11-13 22:09:20.1548 IST [Coverity Connect Scan] INFO: Results are available at https://integrations-qa.dev.cnc.duckutil.net:443/query/defects.htm?stream=build-scan-main&outstanding=true
2025-11-13 22:09:20.1567 IST [Coverity Connect Scan] INFO: Analyze phase took 1m38.615s.
2025-11-13 22:09:20.1575 IST [Coverity Connect Scan] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 22:09:20.1575 IST [Coverity Connect Scan] WARNING: 
2025-11-13 22:09:20.1576 IST [Coverity Connect Scan] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 22:09:20.1576 IST [Coverity Connect Scan] WARNING:   * C#
2025-11-13 22:09:20.1576 IST [Coverity Connect Scan] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 22:09:20.1577 IST [Coverity Connect Scan] INFO: Scan complete.
2025-11-13 22:09:20.1618 IST [Coverity Connect Scan] INFO: Coverity Capture completed successfully
2025-11-13 22:09:20.1709 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.completed'
2025-11-13 22:09:20.1714 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 22:09:20.1735 IST [Coverity Connect Scan] INFO: Adapter finished
2025-11-13 22:09:20.2223 IST [SCM Checker] INFO: Adapter finished
2025-11-13 22:09:21.8180 IST [Coverity Connect Post Scan] INFO: Provided value for resource 'coverity.connect.resultURL'
2025-11-13 22:09:21.8183 IST [Coverity Connect Post Scan] INFO: Provided value for resource 'coverity.connect.policy.issueCount'
2025-11-13 22:09:21.8187 IST [Coverity Connect Post Scan] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 39
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
Configuration: [githubOrg:coverity-cnc-jenkins-samples, repoName:build-scan, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_Coverity_Build_Scan/main
[Pipeline] echo
Build Number: 4
[Pipeline] echo
GitHub Organization: coverity-cnc-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: build-scan
[Pipeline] echo
Target repository: coverity-cnc-jenkins-samples/build-scan
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*