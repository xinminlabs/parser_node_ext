# ParserNodeExt

It assigns names to the child nodes of the [parser](https://rubygems.org/gems/parser).

```ruby
# node is a send node
node.receiver # get the receiver of node
node.message # get the message of node
node.arguments # get the arguments of node
```

It also adds some helpers

```ruby
# node is a hash node
node.foo_pair # get the pair node of hash foo key
node.foo_value # get the value node of the hash foo key
node.foo_source # get the source of the value node of the hash foo key
```

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'parser_node_ext'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install parser_node_ext

## Usage

```ruby
require 'parser/current'
require 'parser_node_ext'
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and the created tag, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/parser_node_ext.
