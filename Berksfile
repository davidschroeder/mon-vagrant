require 'rubygems'

if Gem::Specification::find_by_name('berkshelf').version.to_s[0] == '3'
  source 'https://api.berkshelf.com'
end

cookbook 'mini-mon', path: './cookbooks/mini-mon'
cookbook 'devstack', path: './cookbooks/devstack'
cookbook 'mon_api', git: 'https://github.com/hpcloud-mon/cookbooks-mon_api'
cookbook 'kafka', git: 'https://github.com/hpcloud-mon/cookbooks-kafka'
cookbook 'mon_agent', git: 'https://github.com/hpcloud-mon/cookbooks-mon_agent'
cookbook 'mon_notification', git: 'https://github.com/hpcloud-mon/cookbooks-mon_notification'
cookbook 'mon_persister', git: 'https://github.com/hpcloud-mon/cookbooks-mon_persister.git'
cookbook 'mon_thresh', git: 'https://github.com/hpcloud-mon/cookbooks-mon_thresh'
cookbook 'storm', git: 'https://github.com/tkuhlman/storm'
cookbook 'vertica', git: 'https://github.com/hpcloud-mon/cookbooks-vertica'
cookbook 'zookeeper', git: 'https://github.com/hpcloud-mon/cookbooks-zookeeper'

# The vagrant precise box has an older version of chef when this is fixed we can move to the upstream percona cookbook
#cookbook 'percona', git: 'https://github.com/phlipper/chef-percona'
cookbook 'percona', git: 'https://github.com/tkuhlman/chef-percona', branch: "feature/mini-mon"

# community cookbook we pin, mostly because of the older version of chef in the vagrant precise box
cookbook 'hostsfile', '= 1.0.1'
cookbook 'build-essential', '= 1.4.4'
cookbook 'runit', '= 1.0.4'
cookbook 'sysctl', '= 0.4.0'
cookbook 'openssl', '= 1.1.0'
