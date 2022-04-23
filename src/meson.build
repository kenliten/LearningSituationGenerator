learningsituationgenerator_sources = [
  'main.vala',
  'window.vala',
    'application.vala',
  ]

learningsituationgenerator_deps = [
  dependency('gtk4'),
]

gnome = import('gnome')

learningsituationgenerator_sources += gnome.compile_resources('learningsituationgenerator-resources',
  'learningsituationgenerator.gresource.xml',
  c_name: 'learningsituationgenerator'
)

executable('learningsituationgenerator', learningsituationgenerator_sources,
  vala_args: '--target-glib=2.50',  dependencies: learningsituationgenerator_deps,
  install: true,
)
