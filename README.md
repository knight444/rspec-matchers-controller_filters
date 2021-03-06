# Rspec::Matchers::ControllerFilters

Use this gem to test execution of before/around/after filters of controller actions with RSpec.
http://www.arubystory.com/2014/10/testing-execution-of-beforefilter-with.html

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'rspec-matchers-controller_filters'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install rspec-matchers-controller_filters

## Usage

In your controller specs you may use the new matchers:

```ruby
it { should execute_before_filter :your_filter, :on => :your_action, :with => { :parameter_name => 'parameter_value'} }
it { should_not execute_around_filter :your_filter, :on => :your_action, :with => { :parameter_name => 'parameter_value'} }
it { should execute_after_filter :your_filter, :on => :your_action, :with => { :parameter_name => 'parameter_value'} }
```

The **with** parameter is optional.

## Contributing

1. Fork it ( https://github.com/iridakos/rspec-matchers-controller_filters/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request

## Important note
This is my first gem so please:
1. Use it at your own risk
2. Any feedback is welcome!

##### [**Lazarus Lazaridis**](http://twitter.com/arubystory)
