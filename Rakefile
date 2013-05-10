require 'rake'

task :default => [:install]

task :install do
  destination = ""
  destinations = ["/usr/local/bin", "#{Dir.home}/bin", "#{Dir.home}/home/bin"]
  destinations.each do |location|
    destination = location if Dir.exists?(location)
  end
  
  FileUtils.install "tdo", "#{destination}/tdo", :mode => 0755, :verbose => true
end
