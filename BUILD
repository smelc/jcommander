java_library(
    name = "jcommander",
    srcs = glob(["src/main/java/com/beust/jcommander/**/*.java"]),
    visibility = ["//visibility:public"],
)

java_test(
    name = "jcommander_tests",
    srcs = glob(["src/test/java/com/beust/jcommander/**/*.java"]),
    deps = [":jcommander",
            "@maven//:org_testng_testng",
            "@maven//:com_fasterxml_jackson_core_jackson_core",
            "@maven//:com_fasterxml_jackson_core_jackson_annotations",
           ],
    add_exports = [ "java.base/sun.reflect.annotation" ],

    main_class = "org.testng.TestNG",
    use_testrunner = False,
    resources = glob(["src/test/resources/**"]),
    data = glob(["src/test/resources/testng*.xml"]),
    args = [
      "src/test/resources/testng-single.xml",
      "src/test/resources/testng.xml",
    ],
)
