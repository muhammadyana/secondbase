require 'bundler/gem_tasks'
require 'rake/testtask'

Rake::TestTask.new do |t|
  t.libs = ['lib','test']
  t.test_files = FileList['test/**/*_test.rb']
  t.verbose = true
end

task :default do
  exec 'appraisal update'
  exec 'appraisal rake test'
end
