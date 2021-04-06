# Event Sourcing on Rails - Peer learning group

A fork of kickstarter's minimal event sourcing framework example app (based on their [blog post](https://kickstarter.engineering/event-sourcing-made-simple-4a2625113224)) for use with a peer learning group. At outset this repo contains

- Kickstarter's initial app
- Rspec for testing
- Rubocop config to pacify my text editor
- [Grape API](https://github.com/ruby-grape/grape), initially with a single `POST /api/events` route.

## Usage

Some things you can do right now:

```sh
bundle
bundle exec rake db:setup
bundle exec rails s
```

Make a request

```
POST http://localhost:3000/api/events
{
    "type": "TodoList::Created",
    "body": {"name": "My todos"}
}
```

This project is licensed under the terms of the MIT license.
