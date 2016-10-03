# nsx
A command-line tool to query Google's public DNS over their HTTPS API. The name is inspired by
Acura's awesome NSX.

### API Reference
https://developers.google.com/speed/public-dns/docs/dns-over-https

### Example Usage
```sh
cargo build --release

cargo run --release -- google.com

[
    {
        "name": "google.com.",
        "type": 1,
        "TTL": 299,
        "data": "172.217.4.142"
    }
]
```

### TODO
- Find out a better way to handle query parameters in the curl library.

### License
MIT
