require 'rubygems'
require 'rake'
require 'rake/clean'
require 'bundler'

Bundler.setup

CLEAN.include('build')

directory 'build'

desc 'Package up the xpi'
task :package => [ :build ] do
  Dir.chdir('extension') do
    sh "zip -r ../build/jspec-example.xpi ."
  end
end

task :default => :spec

desc 'Run the specs'
task :spec do

end
