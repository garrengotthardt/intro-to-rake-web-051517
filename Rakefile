desc 'outputs hello to the terminal'
namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hola from the terminal'
  task :hola do
    puts "hola de Rake!"
  end

end


desc 'migrate changes to your database'
namespace :db do
  task :environment do
  require_relative './config/environment'
  end

  task :migrate => :environment do
    Student.create_table
  end

  task :seed do
    require_relative './db/seeds.rb'
  end


end
