# Fuzzing with POST Requests

When fuzzing POST requests, you need to specify the method, data, and optionally, headers.

## Basic POST Example

```bash
./FuzzSwarm -u http://example.com/login -X POST -d 'username=FUZZ&password=password'
```

- `FUZZ` is used in the POST data, and the payloads will come from a wordlist or range.

## Using JSON and Custom Headers

For fuzzing endpoints that accept JSON data, you can set custom headers to specify the content type and send JSON payloads:

```bash
./FuzzSwarm -u http://example.com/login -X POST -H "Content-Type: application/json" -d '{"username": "FUZZ", "password": "password"}'
```

---

Move on to learn about [filters and configuration](advanced/filters_config.md).
