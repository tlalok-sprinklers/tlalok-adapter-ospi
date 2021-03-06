# Tlalok::Adapter::Ospi

[![Gem Version](https://badge.fury.io/rb/tlalok-adapter-ospi.svg)](http://badge.fury.io/rb/tlalok-adapter-ospi)
[![Build Status](https://travis-ci.org/tlalok-sprinklers/tlalok-adapter-ospi.svg?branch=master)](https://travis-ci.org/tlalok-sprinklers/tlalok-adapter-ospi/)
[![Code Climate](https://codeclimate.com/github/tlalok-sprinklers/tlalok-adapter-ospi/badges/gpa.svg)](https://codeclimate.com/github/tlalok-sprinklers/tlalok-adapter-ospi)
[![Dependency Status](https://gemnasium.com/tlalok-sprinklers/tlalok-adapter-ospi.svg)](https://gemnasium.com/tlalok-sprinklers/tlalok-adapter-ospi)

An [OSPI](http://rayshobby.net/ospi/) Adapter for [Tlalok](https://github.com/tlalok-sprinklers)


Can also be used as a stand alone executable, useful if you wanted to cron your sprinklers.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'tlalok-adapter-ospi'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install tlalok-adapter-ospi

## Usage

### CLI

    # this will run station one
    ospi open 1

    # this will stop station one
    ospi close 1

### From the code

```ruby
require 'tlalok/adapter/ospi'

controller = ::Tlalok::Adapter::Ospi::Controller.new

# this will open station 1
controller.open 1

controller.close 1
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake test` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment. Run `bundle exec tlalok-adapter-ospi` to use the gem in this directory, ignoring other installed copies of this gem.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/tlalok-sprinklers/tlalok-adapter-ospi.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
