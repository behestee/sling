package(default_visibility = ["//visibility:public"])

# File system interface.

cc_library(
  name = "file",
  srcs = ["file.cc"],
  hdrs = ["file.h"],
  deps = [
    "//sling/base",
    "//sling/base:registry",
  ],
  copts = [
    "-pthread",
  ],
)

cc_library(
  name = "posix",
  srcs = ["posix.cc"],
  hdrs = ["posix.h"],
  deps = [
    ":file",
    "//sling/base",
  ],
  alwayslink = 1,
)

