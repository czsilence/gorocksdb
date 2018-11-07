# gorocksdb, a Go wrapper for RocksDB

## Install

You'll need to build [RocksDB](https://github.com/facebook/rocksdb) v5.5+ on your machine.

After that, you can install gorocksdb using the following command:

    CGO_CFLAGS="-I/path/to/rocksdb/include" \
    CGO_LDFLAGS="-L/path/to/rocksdb -lrocksdb -lstdc++ -lm -lz -lbz2 -lsnappy -llz4 -lzstd" \
      go get github.com/czsilence/gorocksdb

Please note that this package might upgrade the required RocksDB version at any moment.
Vendoring is thus highly recommended if you require high stability.

*The [embedded CockroachDB RocksDB](https://github.com/cockroachdb/c-rocksdb) is no longer supported in gorocksdb.*
