# safe_app nodejs Change Log

## [0.6.1] - 18-1-2018
## Changed
- Recommend Node ^8.0.0 for building from source
- Upgrade CI scripts to test Node 8.0.0
- Pass the system URI's execution path as an array of arguments to support white spaces in it
- Adapt to changes in `system_uri` library API which now returns results as a pointer to FfiResult struct
- Upgrade system_uri library to v0.4.0

### SAFE libraries Dependencies
- safe_app: v0.5.0
- system_uri: v0.4.0

## [0.6.0] - 20-12-2017
### Added
- Increase test coverage to 90%+ plus minor reorganisation of tests

### Fixed
- Remove '/' characters added by some OS to auth URI before decoding it
- Fix issue in webFetch with URL's ending with '/' to correctly treat it as ending with a folder path

### SAFE libraries Dependencies
- safe_app: v0.5.0
- system_uri: v0.3.0

## 0.5.3
- Fix webFetch to load URLs from root and sub directory

## 0.5.2
- Fix webFetch to load URLs from root and sub directory

## 0.5.1
- Upgrade safe_app version to `57f3afb`
- Adapt to change in safe_app which adds app's ID in unreg auth requests

## 0.5.0

- Add function to retrieve account information
- Adapt to API changes from safe_client_libs to upgrade to latest version
- Add functions to verify network connection state
- Add API to manage signing keys (sign/verify functions included)
- Automate npm publish process triggered upon tag push
- Upgrade system_uri to v0.3.0

## 0.4.1

- Expose Constants which can be used by Apps
- Rely on the safe-core network observer callbacks upon a reconnection
- Uses e9080ac commit version from [alpha-2 branch](https://github.com/maidsafe/safe_client_libs/tree/f40fef47973294b03f8e37dade8edaa8e2da20c9)

## 0.4.0

- Compatible with safe_app v0.4.0
- New set of standalone API Examples Using Mock Routing
- Automatically remove white spaces from appInfo vendor and name to create the .desktop files when registering the URI scheme
- Add an option to allow registration of additional custom protocols in the system URI scheme.
- Support for passing the bundle id in the appInfo object upon initialisation needed for OSX system URI registration
- Upgrade system_uri to v0.2.3

## 0.3.0

- Compatible with safe_app v0.4.0
- Minor fixes
- uses system_uri v0.2.2

## 0.1.0-dev.1

- NFS API updates
- Freeing of safe_app handles
- Minor fixes
