# Karma Query API Client

Python client to query the Karma API.

With this API, you can query the reputation about various asset types (IP, Domain, Website, User) *1

## Example Usage:

```
$ karma 181.64.192.163
{'asn': 6147,
 'asname': 'Telefonica del Peru S.A.A.,PE',
 'blacklists': ['uceprotect.level1',
                'uceprotect.level2',
                'spamhaus.css',
                'sorbs.spam',
                'bad.psky.me'],
 'cc': 'PE',
 'country': 'Peru',
 'rir': 'LACNIC',
 'status': 'blacklisted'}
```

## API KEY

To use the client, you must have a valid Karma API Key.

You can obtain a free API Key on [https://karma.securetia.com](https://karma.securetia.com)

The API Key can be specified as a parameter "-k" or "--key".

Also, can be defined has an environment variable (KARMA_APIKEY).

## Dependencies

This client only depends on Python 3.x, doesn't needs any another package.

## Cache

By default, the client uses a SQLITE database as a cache.

Each entry is cached for 900 seconds (15 minutes).

*1 (now, only the IP query is implemented, but the rest will be implemented in the short time)
