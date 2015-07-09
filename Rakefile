require "bundler/gem_tasks"
require "rspec/core/rake_task"

RSpec::Core::RakeTask.new(:spec)
task :default => :spec


task :rebuild do 
  system "cd ~/code/simplenlg && mvn clean install -DskipTests=true"
  system "cp ~/code/simplenlg/target/SimpleNLG-4.4.7-SNAPSHOT.jar ~/code/simplernlg/lib/jars/"
end

# cd ~/code/simplenlg && mvn clean install -DskipTests=true && cp ~/code/simplenlg/target/SimpleNLG-4.4.7-SNAPSHOT.jar ~/code/simplernlg/lib/jars/ && cd ~/code/simplernlg