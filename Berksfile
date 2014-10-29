source "https://supermarket.getchef.com"

BERKS_DIR = File.expand_path(File.dirname(__FILE__))
LOCAL_COOKBOOKS_DIR = File.join(File.dirname(__FILE__), 'chef/cookbooks')
LOCAL_COOKBOOK_NAMES = Dir.entries(LOCAL_COOKBOOKS_DIR).reject { |e| e.include?('.') }

def add_cookbook(name, opts={})
  path = File.join(LOCAL_COOKBOOKS_DIR, name)
  cookbook name, opts.merge(path: path)
end

LOCAL_COOKBOOK_NAMES.each do |name|
  add_cookbook(name)
end

cookbook 'build-essential'
cookbook 'database', "= 1.3.12"
cookbook 'mysql', "= 2.1.2"
cookbook 'n98-magerun'
cookbook 'newrelic'
cookbook 'nginx'
cookbook 'ntp'
cookbook 'openssh'
cookbook 'php'
cookbook 'php-fpm'
cookbook 'resolver'
cookbook 'rsync'
cookbook 'timezone'
cookbook 'timezone-ii'
cookbook 'users'
cookbook 'vim'
cookbook 'magento'
