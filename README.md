<p align="center">
  <img src="https://example.com/fast-studio.svg" alt="fast-studio" width="200" height="200" />
</p>

<h1 align="center">fast-studio</h1>

<h4 align="center">
  <a href="https://github.com/fast-studio">Repository</a> |
  <a href="https://docs.app">Documentation</a> |
  <a href="https://discord.app">Discord</a> |
  <a href="https://roadmap.app">Roadmap</a>
</h4>

<p align="center">
  <a href="https://github.com/fast-studio/actions"><img src="https://github.com/fast-studio/workflows/Tests/badge.svg" alt="Test"></a>
  <a href="https://badge.fury.io/rb/fast-studio"><img src="https://badge.fury.io/rb/fast-studio.svg" alt="Version"></a>
  <a href="https://github.com/fast-studio/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-informational" alt="License"></a>
</p>

<p align="center">⚡ developer utility for common operations 💎</p>

## 📖 Documentation

Complete usage detailed in this README.

## 🤖 Compatibility

This package guarantees compatibility with version v1.x.

## 📧 Installation

With `gem` in command line:
```bash
gem install fast-studio
```

In your `Gemfile`:
```ruby
gem 'fast-studio'
```

### Run fast-studio

```bash
fast-studio --master-key=masterKey
```

## 🚀 Getting started

#### Configuration

Create `config/initializers/fast-studio.rb`:

```ruby
fast-studio::Config.setup do |config|
  config.api_key = 'YourAPIKey'
  config.url = 'http://localhost:7700'
end
```

#### Add documents

```ruby
client = fast-studio::Client.new
index = client.index('items')

documents = [
  { id: 1, title: 'backups' },
  { id: 2, title: 'swistalongczek' }
]

index.add_documents(documents)
```

## ⚙️ Contributing

Any contribution is welcome!

## 💛 Credits

Inspired by [backups] and [swistalongczek].

