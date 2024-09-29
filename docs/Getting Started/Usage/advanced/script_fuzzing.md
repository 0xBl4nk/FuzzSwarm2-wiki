# Scripted Fuzzing

FuzzSwarm supports custom fuzzing scripts for specific attack types. Currently, it includes an SSTI (Server-Side Template Injection) script.

## Using the SSTI Script

The SSTI script automatically injects payloads designed to exploit template injection vulnerabilities:

```bash
./FuzzSwarm -u http://example.com/vulnerable/FUZZ --script ssti
```
Future updates will introduce more scripts for different attack types.

---
