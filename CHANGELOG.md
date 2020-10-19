warc2zim
===

# 1.2.0

* Accepts directory inputs as well as individual files. If directory given, which will process all .warc and .warc.gz files recursively in the directory.
* If trailing slash is missing on main URL,  `--url https://example.com?test=value`, slash added and URL treated as `--url https://example.com/?test=value`

# 1.1.0

* Now defaults to including all URLs unless --include-domains is specifief (removed `-a`)
* Arguments are now checked before starting. Also returns `100` on valid arguments but no WARC provided.

# 1.0.1

* Now skipping WARC records that redirect to self (http -> https mostly)

# 1.0.0

* Initial release