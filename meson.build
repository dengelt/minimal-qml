project('minimal-qml', 'cpp',
  version : '0.1.0',
  meson_version : '>= 0.37.0',
  default_options: [
    'cpp_std=c++14',
    'warning_level=2',
  ]
)

# Common dependencies
qt5 = import('qt5')
qt5_dep = dependency('qt5', modules: ['Gui', 'Qml', 'WaylandCompositor'])
qrc = qt5.preprocess(qresources: ['minimal-qml.qrc'])

executable('minimal-qml', 'main.cpp', qrc, dependencies : qt5_dep)
