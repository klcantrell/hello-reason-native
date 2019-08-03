# hello-reason-native

### Testing Reason native workflow with esy and pesy

[![CircleCI](https://circleci.com/gh/yourgithubhandle/hello-reason-native/tree/master.svg?style=svg)](https://circleci.com/gh/yourgithubhandle/hello-reason-native/tree/master)

**Contains the following libraries and executables:**

```
hello-reason-native@0.0.0
│
├─test/
│   name:    TestHelloReasonNative.exe
│   main:    TestHelloReasonNative
│   require: hello-reason-native.lib
│
├─library/
│   library name: hello-reason-native.lib
│   namespace:    HelloReasonNative
│   require:
│
└─executable/
    name:    HelloReasonNativeApp.exe
    main:    HelloReasonNativeApp
    require: hello-reason-native.lib
```

## Developing:

```
npm install -g esy
git clone <this-repo>
esy install
esy build
```

## Running Binary:

After building the project, you can run the main binary that is produced.

```
esy x HelloReasonNativeApp.exe
```

## Running Tests:

```
# Runs the "test" command in `package.json`.
esy test
```
