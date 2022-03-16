## Setup

### docker compose

```sh
brew install --cask docker
  
echo "alias dr='docker compose run --rm '" >> ~/.zshrc
```

## Usage

```sh
dr bundle install
dr bundle update some-gem --conservative

docker compose up -d

dr rspec spec
dr rspec spec/some/file_spec.rb:39
```
