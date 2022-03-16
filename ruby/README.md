## Setup

### docker compose

```sh
brew install --cask docker
  
echo "alias dr='docker compose run --rm '" >> ~/.zshrc
```

### env

```sh
export LOCAL_GEM_PATH=~/gems
```

## Usage

### cli

```sh
dr bundle install
dr bundle update some-gem --conservative

docker compose up -d

dr console

dr rspec spec
dr rspec spec/some/file_spec.rb:39
```

### deps

```ruby
# Gemfile

gem "some-gem", path: "/local/some-gem"
```
