source "https://rubygems.org"
gemspec name: "train"

group :test do
  gem "minitest", "~> 5.8"
  gem "rake", "~> 13.0"
  gem "chefstyle", "2.1.1"
  gem "concurrent-ruby", "~> 1.0"
  gem "pry-byebug"
  gem "m"
  gem "ed25519" # ed25519 ssh key support
  gem "bcrypt_pbkdf" # ed25519 ssh key support
  # This is not a true gem installation
  # (Gem::Specification.find_by_path('train-gem-fixture') will return nil)
  # but it's close enough to show the gempath handler can find a plugin
  # See test/unit/
  gem "train-test-fixture", path: "test/fixtures/plugins/train-test-fixture"
  gem "mocha", "~> 2.1"
  gem "simplecov", "~> 0.21"
  gem "simplecov_json_formatter"
end

if Gem.ruby_version >= Gem::Version.new("2.7.0")
  group :integration do
    gem "berkshelf", ">= 6.0"
    gem "test-kitchen", ">= 2"
    gem "kitchen-vagrant"
  end
end

group :tools do
  gem "pry", "~> 0.10"
  gem "rb-readline"
  gem "license_finder"
end
