config_data = configuration_data()

config_data.set('MAJOR_VERSION', MAJOR_VERSION)
config_data.set('MINOR_VERSION', MINOR_VERSION)
config_data.set('PATCH_VERSION', PATCH_VERSION)

config_file = configure_file(
    output: 'config.h',
    configuration: config_data)

config_lib = valac.find_library(
    'config',
    dirs: meson.current_source_dir())

config_dep = declare_dependency(
    dependencies: config_lib,
    include_directories: include_directories('.'))
