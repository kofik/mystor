# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require File.expand_path('../config/application', __FILE__)

Rails.application.load_tasks

require 'sdoc'
namespace :sdoc do
  RDoc::Task.new(:app) do |rdoc|
    rdoc.rdoc_dir = 'doc/app'

    rdoc.options << '-e'  << 'UTF-8'
    rdoc.options << '-f'  << 'sdoc'
    rdoc.options << '-T'  << 'rails'

    rdoc.rdoc_files.include('README.rdoc')
    rdoc.rdoc_files.include('app/**/*.rb')
    rdoc.rdoc_files.include('lib/**/*.rb')
  end
end
