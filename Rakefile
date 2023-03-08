# frozen_string_literal: true

require "bundler/gem_tasks"
require "rspec/core/rake_task"

RSpec::Core::RakeTask.new(:spec)

require "rubocop/rake_task"

RuboCop::RakeTask.new

task default: %i[spec rubocop]

namespace :jp_train_lines_and_stations do
  namespace :data do
    desc 'Updates JP Train Lines and Station data'
    task :update_all do
      puts 'Reset temp DB...'
      # general = Jpostcode::Data::General.new
      # general.reset_table

      # puts 'Retrieveing general zip data...'
      # general.retrieve_and_save

      # puts 'Retrieveing office zip data...'
      # office = Jpostcode::Data::Office.new
      # office.retrieve_and_save

      # puts 'Extract to json files...'
      # Jpostcode::Data::Exporter.new.execute
    end
  end
end
