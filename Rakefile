namespace :greeting do
desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end
end

namespace :greeting do
desc 'outputs hello to the terminal'
task :hola do
  puts "hola de Rake!"
end
end

task :environment do
  require_relative './config/environment'
end

namespace :db do
  task :migrate => :environment do
    Student.create_table
  end
end

namespace :db do 
  task :seed do
    require_relative './db/seeds.rb'
  end
end
