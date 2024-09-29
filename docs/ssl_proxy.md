# SSL and Proxy Setup

FuzzSwarm supports SSL and proxy configurations for more advanced use cases. These settings can be managed through a `.env` file.

## Configuring the .env File

```bash
HTTP_PROXY=http://127.0.0.1:8000
SSL_CERT_PATH=PATH_TO_CERT
```

To use the proxy and SSL features, use the --use-proxy and --use-ssl flags:

```bash
./FuzzSwarm -u http://example.com/api/FUZZ -W wordlist.txt --use-proxy --use-ssl
```

---