desc "Bootstrap the development environment for Recollections development"
task :bootstrap do
  basedir = Dir.pwd
  %x[git submodule init]
  %x[git submodule foreach git fetch]
  %x[git submodule update]
  %x[git submodule foreach git checkout master]

  Dir.glob("*").select { |f| File.directory?(f) }.each do |d|
    Dir.chdir(d)
    %x[rake bootstrap] if File.exists?('Rakefile')
    Dir.chdir(basedir)
  end
end

task :default => :bootstrap
