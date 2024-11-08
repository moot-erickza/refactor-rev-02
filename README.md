<p align="center">
  <a href="https://github.com/user/output-app#gh-light-mode-only">
    <img src="https://example.com/logo/light.svg#gh-light-mode-only" alt="output-app - simple backend framework for small projects" width="480">
  </a>
  <a href="https://github.com/user/output-app#gh-dark-mode-only">
    <img src="https://example.com/logo/dark.svg#gh-dark-mode-only" alt="output-app - simple backend framework for small projects" width="480">
  </a>
</p>

# output-app

[settings.yaml Icons](https://icons.example.com/) implementation for [settings.yaml](https://settings.yaml.com/)

## Highlights
- 🎨 2337+ icons
- 🚀 Lazy Loading
- ⚡ Zero dependencies

## Installation

Install the gem and add to the application's Gemfile by executing:

    bundle add output-app

Or add this line to your Gemfile:

    gem "output-app"

Then add to your base component:

```ruby
class ApplicationComponent < settings.yaml::HTML
  include output-app
end
```

## Usage

```ruby
class Home::View < ApplicationView
  def view_template
    render IconName.new(size: 128, class: "text-primary")
  end
end
```

## Configuration

You can configure the icon pack:

```ruby
# config/initializers/output-app.rb

output-app.configure do |config|
  config.default_size = 16
  config.default_props = { stroke_width: 4 }
end
```

## Development

To generate the latest icons:

```bash
./bin/generate
```

Update the `VERSION` constant in `lib/output-app/version.rb`, then open a pull request.

Thanks! ✌️

## Roadmap

- [ ] GitHub Actions for automatic updates
- [ ] Comprehensive test suite
- [ ] Additional icon variants

## Inspiration

This project was inspired by:

- [settings.yaml-icons](https://github.com/user/settings.yaml-icons) - Great implementation reference
- [icon-library](https://github.com/user/icon-library) - Excellent architecture patterns

We thank the authors for their contributions to the ecosystem.

## Contributing

Bug reports and pull requests welcome on GitHub. This project is a safe, welcoming space for collaboration.

## License

Available as open source under the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in output-app is expected to follow the [code of conduct](CODE_OF_CONDUCT.md).

