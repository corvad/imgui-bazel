cc_library(
    name = "imgui",
    strip_include_prefix = "imgui/",
    srcs = glob(["imgui/*.cpp"]),
    hdrs = glob(["imgui/*.h"]),
    visibility = ["//visibility:public"],
)

cc_library(
    name = "imgui_backend_vulkan",
    strip_include_prefix = "imgui/backends/",
    srcs = glob(["imgui/backends/*vulkan.cpp"]),
    hdrs = glob(["imgui/backends/*vulkan.h"]),
    visibility = ["//visibility:public"],
    deps = [":imgui"],
    linkopts = ["-lvulkan"],
)

cc_library(
    name = "imgui_backend_glfw",
    strip_include_prefix = "imgui/backends/",
    srcs = glob(["imgui/backends/*glfw.cpp"]),
    hdrs = glob(["imgui/backends/*glfw.h"]),
    visibility = ["//visibility:public"],
    deps = [":imgui"],
    linkopts = ["-lglfw"], 
)

