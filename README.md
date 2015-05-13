## Sensu-Plugins-eep

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-eep.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-eep)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-eep.svg)](http://badge.fury.io/rb/sensu-plugins-eep)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-eep/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-eep)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-eep/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-eep)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-eep.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-eep)
[ ![Codeship Status for sensu-plugins/sensu-plugins-eep](https://codeship.com/projects/5a5f3be0-db3a-0132-cb23-0eed4ec53b27/status?branch=master)](https://codeship.com/projects/79571)

## Functionality

## Files
 * bin/handler-eep

## Usage

```
{
  "eep": {
    "api_token": "API_TOKEN"
  }
}
```

## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-eep -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-eep`

#### Bundler

Add *sensu-plugins-eep* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-eep' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-eep' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
