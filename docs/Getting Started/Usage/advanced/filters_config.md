# Filters and Advanced Configuration

FuzzSwarm offers several options to filter responses and optimize performance:

## Response Filtering

- **--filter-size** or **-f**: Filter responses by size.

Example:

```bash
./FuzzSwarm -u http://example.com/api/FUZZ -W wordlist.txt -f 200
```
This will only display responses that are not 200 bytes.

### Verbose Output
To see full response bodies, use the --verbose flag:
```bash
./FuzzSwarm -u http://example.com/api/FUZZ -W wordlist.txt --verbose
```

### Threads and Timeout

- `--threads or -t`: Set the number of threads to use.
= `--timeout`: Set the timeout for requests in seconds.

Example with multiple threads and a 5-second timeout:

```bash
./FuzzSwarm -u http://example.com/api/FUZZ -W wordlist.txt --threads 10 --timeout 5
```

---

Read about [scripted fuzzing](script_fuzzing.md) for more advanced usage.
