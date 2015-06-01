# -*- coding: utf-8 -*-

# css 生成用
compass_options = {
  project_path:       'assets',
  configuration_file: 'assets/config.rb',
  patterns: [%r{^assets/sass/(.*)\.s[ac]ss$}]
}
guard :compass, compass_options do
  compass_options[:patterns].each { |pattern| watch(pattern) }
end

# js 生成用
coffeescript_options = {
  input:  'assets/coffee',
  output: 'assets/js',
  patterns: [%r{^assets/coffee/(.+\.(?:coffee|coffee\.md|litcoffee))$}]
}

guard :coffeescript, coffeescript_options do
  coffeescript_options[:patterns].each { |pattern| watch(pattern) }
end

# html 生成用
haml_options = {
  input:  'assets',
  output: 'assets',
  patterns: [%r{^assets/(.+\.haml)$}]
}

guard :haml, haml_options do
  haml_options[:patterns].each { |pattern| watch(pattern) }
end

