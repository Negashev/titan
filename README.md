# Titan

[![Build Status](https://travis-ci.org/distributedio/titan.svg?branch=master)](https://travis-ci.org/distributedio/titan)
[![Go Report Card](https://goreportcard.com/badge/github.com/distributedio/titan)](https://goreportcard.com/report/github.com/distributedio/titan)
[![Coverage Status](https://coveralls.io/repos/github/distributedio/titan/badge.svg?branch=master)](https://coveralls.io/github/distributedio/titan?branch=master)
[![Coverage Status](https://img.shields.io/badge/version-v0.3.1-brightgreen.svg)](https://github.com/distributedio/titan/releases)
[![Discourse status](https://img.shields.io/discourse/https/meta.discourse.org/status.svg)](https://titan-tech-group.slack.com)

A distributed implementation of Redis compatible layer based on [TiKV](https://github.com/tikv/tikv/)
## Features

* Completely compatible with redis protocol
* Full distributed transaction with strong consistency
* Multi-tenancy support
* No painful scale out
* High availability 

Thanks [TiKV](https://github.com/tikv/tikv/) for supporting the core features 

## Roadmap

[Roadmap](docs/roadmap.md)

## Can't wait to experiment Titan?

```
curl -s -O https://raw.githubusercontent.com/distributedio/titan/master/docker-compose.yml
docker-compose up

# Then connect to titan use redis-cli
redis-cli -p 7369

# Enjoy!
```

## Installing

[Deploy Titan](docs/ops/deploy.md)

## Benchmarks

[Titan Benchmarks](docs/benchmark/benchmark.md)

## FAQ

[FAQ](https://github.com/distributedio/titan/issues?utf8=%E2%9C%93&q=+label%3A%22good+first+issue%22)

## Commands

### Connections
- [x] auth 
- [x] echo 
- [x] ping
- [x] quit 
- [x] select 
- [ ] swapdb, not supported

### Transactions
- [x] multi 
- [x] exec
- [x] discard
- [x] watch
- [x] unwatch

### Server
- [x] client list
- [x] client kill
- [x] client pause
- [x] client reply 
- [x] client getname
- [x] client setname
- [x] monitor
- [x] debug object
- [x] flushdb
- [x] flushall
- [x] time
- [x] command
- [x] command count
- [x] command getkeys
- [x] command info
- [x] info
- [ ] slowlog

### Keys
- [x] del 
- [x] type
- [x] exists
- [x] expire
- [x] expireat
- [x] object 
- [x] pexpire
- [x] pexpireat
- [x] ttl
- [x] pttl
- [x] randomkey
- [ ] touch 
- [x] keys
- [x] scan
- [ ] unlink

### Strings

- [x] get 
- [x] set 
- [x] mget 
- [x] mset 
- [x] strlen
- [x] incr
- [x] incrby
- [x] decr
- [x] decrby
- [x] append
- [ ] bitcount
- [ ] bitfield
- [ ] bitop
- [ ] bitpos
- [ ] getbit
- [x] getrange
- [x] getset
- [x] incrbyfloat 
- [ ] msetnx
- [x] psetex
- [ ] setbit
- [x] setex
- [x] setnx
- [ ] setrange

### List

- [x] lrange
- [x] linsert
- [x] lindex
- [x] llen
- [x] lset
- [x] lpush
- [x] lpop
- [x] lpushx
- [ ] ltrim
- [ ] lrem
- [ ] rpop
- [ ] rpoplpush
- [x] rpush
- [ ] rpushhx
- [ ] blpop
- [ ] brpop
- [ ] brpoplpush

### Hashes
- [x] hset
- [x] hget
- [x] hgetall
- [x] hdel
- [x] hexists
- [x] hincrby
- [x] hincrbyfloat
- [x] hkeys
- [x] hlen
- [x] hmget
- [x] hmset
- [x] hscan
- [x] hsetnx
- [x] hstrlen
- [x] hvals

### Sets

- [ ] sadd
- [ ] scard
- [ ] sdiff
- [ ] sdiffstore
- [ ] sinter
- [ ] sinterstore
- [ ] sismember
- [ ] smembers
- [ ] smove
- [ ] spop
- [ ] srandmember
- [ ] srem
- [ ] sunion
- [ ] sunionstore
- [ ] sscan

### Sorted Sets

- [ ] bzpopmin
- [ ] bzpopmax
- [x] zadd
- [x] zcard
- [ ] zcount
- [ ] zincrby
- [ ] zinterstore
- [ ] zlexcount
- [ ] zpopmax
- [ ] zpopmin
- [x] zrange
- [ ] zrangebylex
- [ ] zrevrangebylex
- [ ] zrangebyscore
- [ ] zrank
- [x] zrem
- [ ] zremrangebylex
- [ ] zremrangebyrank
- [ ] zremrangebyscore
- [x] zrevrange
- [ ] zrevrangebyscore
- [ ] zrevrank
- [x] zscore
- [ ] zunionstore
- [ ] zscan

### Geo

- [ ] geoadd
- [ ] geohash
- [ ] geopos
- [ ] geodist
- [ ] georadius
- [ ] georadiusbymember

### hyperloglog

- [ ] pfadd
- [ ] pfcount
- [ ] pfmerge

### Pub/Sub

- [ ] psubscribe
- [ ] pubsub
- [ ] publish
- [ ] punsubscribe
- [ ] subscribe
- [ ] unsubscribe

### Scripting

- [x] eval
- [ ] evalsha
- [ ] script debug
- [ ] script exists
- [ ] script flush
- [ ] script kill
- [ ] script load

### Streams

- [ ] xadd
- [ ] xrange
- [ ] xrevrange
- [ ] xlen
- [ ] xread
- [ ] xreadgroup
- [ ] xpending
