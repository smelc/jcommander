java_library(
    name = "jcommander",
    srcs = glob(["src/main/java/com/beust/jcommander/**/*.java"]),
    visibility = ["//visibility:public"],
)

java_test(
    name = "jcommander_tests",
    srcs = glob(["src/test/java/com/beust/jcommander/**/*.java"]),
    deps = [":jcommander"],
    # Update this to your actual test class if needed
    test_class = "com.beust.jcommander.JCommanderTest",
)
