desc "Test sudoers syntax"
task :sudoers do
  sh '
if [ "`uname -s`" != Darwin ] && [ "`lsb_release -i | cut -f 2`" = Ubuntu ]; then
    visudo -c -f files/sudoers
fi'
end

task :default => :sudoers
