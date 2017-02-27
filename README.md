Docker memcached-tool
--

Available from docker hub as koudaiii/memcached-tool

## Usage

```bash
$ docker run koudaiii/memcached-tool
Usage: memcached-tool <host[:port] | /path/to/socket> [mode]

       memcached-tool 10.0.0.5:11211 display    # shows slabs
       memcached-tool 10.0.0.5:11211            # same.  (default is display)
       memcached-tool 10.0.0.5:11211 stats      # shows general stats
       memcached-tool 10.0.0.5:11211 settings   # shows settings stats
       memcached-tool 10.0.0.5:11211 sizes      # shows sizes stats
       memcached-tool 10.0.0.5:11211 dump       # dumps keys and values

WARNING! sizes is a development command.
As of 1.4 it is still the only command which will lock your memcached instance for some time.
If you have many millions of stored items, it can become unresponsive for several minutes.
Run this at your own risk. It is roadmapped to either make this feature optional
or at least speed it up.
```
