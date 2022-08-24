# How to connect to school wifi on a Raspberry Pi

This guide will explain how to connect to school wifi on a Pi.

First you will need to generate a hash of the passowrd you use to log on to school wifi. This is a cryptographically secure hash, so others will not be able to access your password from the hash alone.

To do this run this command:

```sh
echo -n YOURPASSWORD | iconv -t utf16le | openssl md4
```

Replace YOURPASSWORD with your actual password.
