# Installation Troubleshooting

## Problems with psycopg2 package installation on Mac
1. First, check that you have postgres and openssl installed
- `brew install openssl` or `brew reinstall openssl`
- `brew install postgresql` or `brew reinstall postgresql`
2. If that doesn't help, try the following:
- `xcode-select --install`
- `env LDFLAGS="-I/usr/local/opt/openssl/include -L/usr/local/opt/openssl/lib" pip install psycopg2`
