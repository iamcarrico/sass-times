require "bundler"
Bundler.setup

task :default => [:test]

task :test do
  require 'compass'
  require 'compass/exec'

  Compass.add_configuration 'config.rb'
  Compass.configuration.project_path = Dir.pwd
  Compass.sass_compiler.clean!
  Compass.sass_compiler({ :time => true }).compile!
end
