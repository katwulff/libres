project(
    'libres',
    ['c', 'vala'],
    version: '0.1.0',
    meson_version: '>= 0.50.0',
    default_options: [
        'warning_level=3',
        'werror=true',
        'optimization=3',
    ],
)

version_split = meson.project_version().split('.')
MAJOR_VERSION = version_split[0]
MINOR_VERSION = version_split[1]
PATCH_VERSION = version_split[2]

cc = meson.get_compiler('c')
valac = meson.get_compiler('vala')

glib_dep = dependency('glib-2.0', version: '>= 2.50')
gobject_dep = dependency('gobject-2.0', version: '>=2.50')
m_dep = cc.find_library('m')

subdir('src')

