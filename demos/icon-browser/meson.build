iconbrowser_sources = [
  'main.c',
  'iconbrowserapp.c',
  'iconbrowserwin.c',
  'iconstore.c'
]

iconbrowser_resources = gnome.compile_resources('iconbrowser_resources',
                                                'iconbrowser.gresource.xml',
                                                source_dir: '.')

executable('gtk4-icon-browser',
           iconbrowser_sources, iconbrowser_resources,
           dependencies: libgtk_dep,
           include_directories: confinc,
           gui_app: true,
           link_args: extra_demo_ldflags,
           install: true)

install_data('org.gtk.IconBrowser.desktop', install_dir: gtk_applicationsdir)