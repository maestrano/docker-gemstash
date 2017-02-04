# Gemstash
Gemstash server

## Examples
```
# Launch gemstash
docker run -d -p '9292:9292' --name gemstash maestrano/gemstash
```

```
# Configure bundler
bundle config mirror.https://rubygems.org http://localhost:9292
bundle config mirror.https://rubygems.org.fallback_timeout 3
```

Remove the bundler mirror after container destruction
```
bundle config --delete mirror.https://rubygems.org
```
