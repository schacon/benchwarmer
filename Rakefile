require 'rubygems'
require 'rake/gempackagetask'
load File.join(File.dirname(__FILE__), 'benchwarmer.gemspec')

Rake::GemPackageTask.new(GEMSPEC).define

task :install => [:package] do
  sh %{sudo gem install pkg/#{GEM}-#{VERSION}}
end
