# Basic Usage

In its simplest form, FuzzSwarm requires the following parameters:

- **--url** or **-u**: The target URL.
- **--wordlist** or **-W**: The path to a wordlist file for fuzzing.
- **--range** or **-R**: An alternative to wordlists, a numeric range for fuzzing.

## Example: Fuzzing a GET Endpoint with a Wordlist

```bash
./FuzzSwarm -u http://example.com/api/endpoint/FUZZ -W wordlist.txt
```

- FUZZ is the placeholder in the URL that will be replaced by each entry in the wordlist.

## Example: Fuzzing a GET Endpoint with a Numeric Range

```bash
./FuzzSwarm -u http://example.com/api/endpoint/FUZZ -R 1-1000,3
```

-  `1-1000` defines the range of numbers to test.
-  `,3` formats the numbers with leading zeros (e.g., 001, 002, etc.).

---

Learn how to perform [POST request fuzzing](fuzzing_post.md).