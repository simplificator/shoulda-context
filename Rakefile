require 'bundler/setup'
require 'bundler/gem_tasks'
require 'rake/testtask'

$LOAD_PATH.unshift("lib")
load 'tasks/shoulda.rake'

Rake::TestTask.new do |t|
  t.libs << 'lib' << 'test'
  test.test_files = FileList['test/test_*.rb']
  t.verbose = false
end

desc 'Default: run tests'
task :default => [:test]
