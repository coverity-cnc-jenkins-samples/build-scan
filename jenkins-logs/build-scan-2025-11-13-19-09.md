# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Coverity_Build_Scan/main`
- **Build Number:** #2
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 3 min 6 sec and counting
- **Timestamp:** 2025-11-13 19:09:36 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from d015cb1e15735cd60950f0b172ee59370dad09ca
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
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/coverity-cnc-jenkins-samples/build-scan.git
 > git init /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2 # timeout=10
Fetching upstream changes from https://github.com/coverity-cnc-jenkins-samples/build-scan.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/coverity-cnc-jenkins-samples/build-scan.git +refs/heads/main:refs/remotes/origin/main # timeout=10
 > git config remote.origin.url https://github.com/coverity-cnc-jenkins-samples/build-scan.git # timeout=10
Avoid second fetch
Checking out Revision d015cb1e15735cd60950f0b172ee59370dad09ca (main)
Commit message: "Coverity Build Scan"
First time build. Skipping changelog.
 > git config --add remote.origin.fetch +refs/heads/main:refs/remotes/origin/main # timeout=10
 > git config core.sparsecheckout # timeout=10
 > git checkout -f d015cb1e15735cd60950f0b172ee59370dad09ca # timeout=10
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
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm
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

added 962 packages, and audited 1412 packages in 14s

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
[Pipeline] { (coverity-build-scan)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm
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
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage connect --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/coverity_input15170920545235892255.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 19:07:00.1525 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 19:07:00.1601 IST [Bridge CLI] INFO: Found version "3.0.128" in registry for workflow "connect", trying to load it from local cache
2025-11-13 19:07:00.2153 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 19:07:00.2153 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 19:07:00.2153 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 19:07:00.2154 IST [Bridge CLI] INFO: coverity.connect.project.name = build-scan [coverity_input15170920545235892255.json]
2025-11-13 19:07:00.2154 IST [Bridge CLI] INFO: coverity.connect.stream.name = build-scan-main [coverity_input15170920545235892255.json]
2025-11-13 19:07:00.2154 IST [Bridge CLI] INFO: coverity.connect.url = https://integrations-qa.dev.cnc.duckutil.net [coverity_input15170920545235892255.json]
2025-11-13 19:07:00.2154 IST [Bridge CLI] INFO: coverity.connect.user.name = admin [coverity_input15170920545235892255.json]
2025-11-13 19:07:00.2154 IST [Bridge CLI] INFO: coverity.connect.user.password = ***************************************** [coverity_input15170920545235892255.json]
2025-11-13 19:07:00.2154 IST [Bridge CLI] INFO: coverity.waitForScan = true [coverity_input15170920545235892255.json]
2025-11-13 19:07:00.2154 IST [Bridge CLI] INFO: network.airgap = false [coverity_input15170920545235892255.json]
2025-11-13 19:07:00.2154 IST [Bridge CLI] INFO: network.ssl.trustAll = false [coverity_input15170920545235892255.json]
2025-11-13 19:07:00.2154 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 19:07:00.2154 IST [Bridge CLI] INFO: Starting adapters for stage connect
2025-11-13 19:07:00.2157 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Controller
2025-11-13 19:07:00.2190 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 19:07:00.2569 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 19:07:00.2572 IST [Check pull request] INFO: Adapter finished
2025-11-13 19:07:04.5609 IST [Coverity Connect Controller] INFO: No coverity version is configured, will use the default or latest supported version from the server
2025-11-13 19:07:04.6475 IST [Coverity Connect Controller] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 19:07:04.6475 IST [Bridge CLI] INFO: Starting adapters for stage connect-post-processing
2025-11-13 19:07:04.6475 IST [Bridge CLI] INFO: Starting adapters for stage scm
2025-11-13 19:07:04.6476 IST [Bridge CLI] INFO: Starting adapters for stage connect-scan
2025-11-13 19:07:04.6479 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Scan
2025-11-13 19:07:04.6480 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Post Scan
2025-11-13 19:07:04.6480 IST [Bridge CLI] INFO: Starting Adapter: SCM Checker
2025-11-13 19:07:04.6482 IST [Coverity Connect Controller] INFO: Adapter finished
2025-11-13 19:07:04.6518 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for Set Version for Coverity
2025-11-13 19:07:04.6519 IST [Default Adapter for Set Version for Coverity] INFO: Provided value for resource 'coverity.version'
2025-11-13 19:07:04.6520 IST [Default Adapter for Set Version for Coverity] INFO: Adapter finished
2025-11-13 19:07:04.7404 IST [Coverity Connect Scan] INFO: Identified workflow: Coverity
2025-11-13 19:07:04.7405 IST [Coverity Connect Scan] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity scan --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -o analyze.location=connect -o commit.connect.url=https://integrations-qa.dev.cnc.duckutil.net -o commit.connect.stream=build-scan-main -o commit.connect.project=build-scan
2025-11-13 19:07:04.7962 IST [Coverity Connect Scan] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 19:07:04.7977 IST [Coverity Connect Scan] WARNING: No setting for 'commit.connect.on-new-cert' specified.
2025-11-13 19:07:04.7977 IST [Coverity Connect Scan] WARNING: Using default value of 'distrust'.
2025-11-13 19:07:04.7977 IST [Coverity Connect Scan] WARNING: This may result in a certificate validation error when uploading defects to Coverity Connect.
2025-11-13 19:07:04.7978 IST [Coverity Connect Scan] WARNING: If you trust the Coverity Connect instance and certificate validation fails, set 'commit.connect.on-new-cert' to 'trust'.
2025-11-13 19:07:04.7978 IST [Coverity Connect Scan] WARNING: If you are unfamiliar with what this means, please talk to your Coverity Connect administrator.
2025-11-13 19:07:04.8044 IST [Coverity Connect Scan] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 19:07:04.8044 IST [Coverity Connect Scan] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 19:07:04.8058 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir create
2025-11-13 19:07:07.3311 IST [Coverity Connect Scan] INFO: Creating stream 'build-scan-main'.
2025-11-13 19:07:08.1068 IST [Coverity Connect Scan] INFO: Cloud analysis is enabled.
2025-11-13 19:07:11.2887 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 19:07:12.1349 IST [Coverity Connect Scan] INFO: Caching is enabled.
2025-11-13 19:07:13.5315 IST [Coverity Connect Scan] INFO: Telemetry is enabled
2025-11-13 19:07:14.0868 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 19:07:14.1031 IST [Coverity Connect Scan] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 19:07:14.6218 IST [Coverity Connect Scan] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir'
2025-11-13 19:07:14.6220 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 19:07:14.8939 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 19:07:15.1839 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 19:07:15.4315 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 19:07:15.6676 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 19:07:15.9169 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 19:07:16.1589 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 19:07:16.4053 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 19:07:16.6551 IST [Coverity Connect Scan] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 19:07:16.6551 IST [Coverity Connect Scan] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 19:07:16.6551 IST [Coverity Connect Scan] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 19:07:16.6601 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 19:07:16.9165 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 19:07:17.2603 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 19:07:17.5040 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 19:07:17.7525 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 19:07:17.9942 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 19:07:18.0129 IST [Coverity Connect Scan] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 19:07:18.0129 IST [Coverity Connect Scan] INFO:           and it will not be updated.
2025-11-13 19:07:18.6076 IST [Coverity Connect Scan] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 19:07:19.2419 IST [Coverity Connect Scan] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 19:07:19.8608 IST [Coverity Connect Scan] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/capture-file-list-3304417767 --record-with-source
2025-11-13 19:07:19.8716 IST [Coverity Connect Scan] INFO: Buildless capture started.
2025-11-13 19:07:19.8817 IST [Coverity Connect Scan] INFO: Emitting 84 Files.
2025-11-13 19:07:20.3305 IST [Coverity Connect Scan] INFO: Buildless capture completed.
2025-11-13 19:07:20.3326 IST [Coverity Connect Scan] INFO: Executing action No unwanted TUs to delete
2025-11-13 19:07:20.3327 IST [Coverity Connect Scan] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 19:07:20.3328 IST [Coverity Connect Scan] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir
2025-11-13 19:07:20.3331 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 19:07:20.3515 IST [Coverity Connect Scan] INFO: Executing action Invalidate capture results
2025-11-13 19:07:20.8800 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 19:07:20.9348 IST [Coverity Connect Scan] INFO: Capture summary:
2025-11-13 19:07:20.9348 IST [Coverity Connect Scan] INFO:     SUCCEEDED: 84
2025-11-13 19:07:20.9348 IST [Coverity Connect Scan] INFO:     INCOMPLETE: 0
2025-11-13 19:07:20.9349 IST [Coverity Connect Scan] INFO:     FAILED: 0
2025-11-13 19:07:20.9349 IST [Coverity Connect Scan] INFO:     IGNORED: 6
2025-11-13 19:07:20.9349 IST [Coverity Connect Scan] INFO:     FILES CAPTURED: 84
2025-11-13 19:07:20.9349 IST [Coverity Connect Scan] INFO:     LINES OF CODE: 32728
2025-11-13 19:07:20.9369 IST [Coverity Connect Scan] INFO: Capture phase took 7.406s.
2025-11-13 19:07:20.9370 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml'
2025-11-13 19:07:20.9394 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/_Github_Coverity_Build_Scan_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml'
2025-11-13 19:07:20.9406 IST [Coverity Connect Scan] INFO: Analyzing project in the cloud using Coverity Analysis version 2025.9.0
2025-11-13 19:07:21.2522 IST [Coverity Connect Scan] INFO: Creating archive containing data to be analyzed...
2025-11-13 19:07:21.2825 IST [Coverity Connect Scan] INFO: Properties archive created.
2025-11-13 19:07:21.2825 IST [Coverity Connect Scan] INFO: Uploading data for analysis...
2025-11-13 19:07:21.9951 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 19:07:27.7248 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 19:07:27.7248 IST [Coverity Connect Scan] INFO: Scan created.
2025-11-13 19:07:27.7248 IST [Coverity Connect Scan] INFO: The scan ID is 'd5b58312-f3a6-4d8d-89a3-c3929b521c1c'
2025-11-13 19:07:27.7251 IST [Coverity Connect Scan] INFO: Waiting for scan to complete...
2025-11-13 19:07:27.7251 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 19:09:30.7161 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 19:09:31.4161 IST [Coverity Connect Scan] INFO: Analysis summary after merging defects:
2025-11-13 19:09:31.4162 IST [Coverity Connect Scan] INFO:     HIGH SEVERITY:    2 issue(s)
2025-11-13 19:09:31.4162 IST [Coverity Connect Scan] INFO:     MEDIUM SEVERITY: 12 issue(s)
2025-11-13 19:09:31.4163 IST [Coverity Connect Scan] INFO:     LOW SEVERITY:    25 issue(s)
2025-11-13 19:09:31.4163 IST [Coverity Connect Scan] INFO:     AUDIT SEVERITY:   0 issue(s)
2025-11-13 19:09:31.4163 IST [Coverity Connect Scan] INFO: Results are available at https://integrations-qa.dev.cnc.duckutil.net:443/query/defects.htm?stream=build-scan-main&outstanding=true
2025-11-13 19:09:31.4388 IST [Coverity Connect Scan] INFO: Analyze phase took 2m10.478s.
2025-11-13 19:09:31.4397 IST [Coverity Connect Scan] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 19:09:31.4397 IST [Coverity Connect Scan] WARNING: 
2025-11-13 19:09:31.4398 IST [Coverity Connect Scan] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 19:09:31.4398 IST [Coverity Connect Scan] WARNING:   * C#
2025-11-13 19:09:31.4398 IST [Coverity Connect Scan] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 19:09:31.4398 IST [Coverity Connect Scan] INFO: Scan complete.
2025-11-13 19:09:31.4424 IST [Coverity Connect Scan] INFO: Coverity Capture completed successfully
2025-11-13 19:09:31.4458 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.completed'
2025-11-13 19:09:31.4459 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 19:09:31.4462 IST [Coverity Connect Scan] INFO: Adapter finished
2025-11-13 19:09:32.9556 IST [SCM Checker] INFO: Adapter finished
2025-11-13 19:09:34.8472 IST [Coverity Connect Post Scan] INFO: Provided value for resource 'coverity.connect.resultURL'
2025-11-13 19:09:34.8475 IST [Coverity Connect Post Scan] INFO: Provided value for resource 'coverity.connect.policy.issueCount'
2025-11-13 19:09:34.8499 IST [Coverity Connect Post Scan] INFO: Adapter finished
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
Build Number: 2
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