# Office of the CTO

Thoughts and ramblings on the mistakes of yesterday and the potential for a better tomorrow.

## Development Environment

1. Adopt [12 Factor](http://12factor.net) from the start
2. Consider using [Boxen](https://github.com/boxen/our-boxen) for new machine configuration
3. Matching Development with Production, lots of options
  1. Use [Heroku pipelines](https://devcenter.heroku.com/articles/pipelines)
  2. Use a managed service like [Nitrous](https://www.nitrous.io) and automate development builds from the beginning
  3. Use [Convox](http://convox.com)
  4. Use [Otto](https://www.ottoproject.io)
4. Sprint Planning [Sprintly](https://sprint.ly)
  
## Architecture

1. Rails 5
  1. Rack middleware for compression, SSL, etc.
    1. [compression](http://www.rubydoc.info/github/rack/rack/master/Rack/Deflater)
  2. [Moneta](https://github.com/minad/moneta) for caching / unified KV interface
  3. Background jobs, [Que](https://github.com/chanks/que)
2. Postgres
3. Redis if necessary
4. JavaScript
  1. TurboLinks
  2. ZeptoJS
  3. [Paloma](https://github.com/kbparagua/paloma)
  4. [React-Rails](https://github.com/reactjs/react-rails)
5. API
  1. Seperate namespace for external API
  2. Seperate namespace for internal API
  3. Use [JSONAPI](https://github.com/cerebris/jsonapi-resources)
6. Styles
  1. Bootstrap 4
  2. SASS
  3. [FontAwesome](http://fontawesome.io) (maybe SVG)
