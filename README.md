# fasjson-client

A python client library for the FASJSON API

This client uses the bravado library to build dynamic api methods based on open-api specs (version 2.0): https://github.com/Yelp/bravado

## Usage

```
c = Client.from_url('http://myspecurl.com', base_url='http://fasjson.example.test/fasjson' principal='admin@EXAMPLE.TEST')

output = c.me.whoami().response().result

print(output)
```

## Development

Install dependencies:

```
pip install -U -r requirements.txt
```

Running tests:

```
pytest
```

## License

Licensed under [lgpl-3.0](./LICENSE)