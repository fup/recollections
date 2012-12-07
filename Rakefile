desc "Bootstrap the development environment for Recollections development"
task :bootstrap do
  %x[git submodule init]
  %x[git submodule foreach git fetch]
  %x[git submodule update]
end

task :default => :bootstrap
