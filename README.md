# KUnit Documentation

KUnit is a lightweight unit testing and mocking framework for the Linux kernel.
These tests are able to be run locally on a developer’s workstation without a VM
or special hardware.

KUnit is heavily inspired by JUnit, Python’s unittest.mock, and
Googletest/Googlemock for C++. KUnit defines a way to mock out C style classes
and functions and create expectations on methods called within the code under
test.

This is a repository to host KUnit project documentation.

## Where is the code?

<https://kunit.googlesource.com>

## Updating this repository

To update the documents in this repository, checkout
<https://kunit.googlesource.com/linux/+/kunit/alpha/master>. Compile the
kernel-docs, and copy them to the kernel-docs repo in this repository:

```bash
git clone https://github.com/google/kunit-docs.git
git clone https://kunit.googlesource.com/linux $PATH_TO_KUNIT_KERNEL
cd kunit-docs
cp -r $PATH_TO_KUNIT_KERNEL/LICENSES/ third_party/kernel/
cp -r $PATH_TO_KUNIT_KERNEL/Documentation/output/ third_party/kernel/docs/
```

