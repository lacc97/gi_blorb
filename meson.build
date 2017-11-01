project('gi_blorb', 'c', version : '1.6.0')

pkg = import('pkgconfig')

gi_blorb_lib = static_library('gi_blorb', 'gi_blorb.c', install : true, install_dir : get_option('libdir') + 'glk/blorb')
install_headers('gi_blorb.h', subdir : 'glk/blorb')
pkg.generate(
    name :          'gi_blorb',
    description :   'Glk blorb layer',
    version :       meson.project_version(),
    subdirs :       'glk/blorb',
    libraries :     gi_blorb_lib
)
