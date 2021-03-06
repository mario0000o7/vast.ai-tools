# Vast.ai tools

This repository will be updated with scripts and other assets used for managing vast.ai servers.

## Analytics dashboard

This is an analytics dashboard for remotely monitoring system information as well as tracking earnings.

[Link to read more](./analytics)

## GPU Profile switcher

Lets you create profiles for power limit, fan speed and clocks. Have a default one for renters and container specific ones for your jobs.

[Link to read more](./gpu-profile)

## Uptime monitor

Receive messages via Telegram if your machine goes down

[Link to read more](./uptime-monitor)

## Stats

Aggregated stats on all active machines

[Link to read more](./stats)

## Benchmarking

Useful commands for benchmarking

[Link to read more](./benchmark)

## Dockerfile.miner

This is the dockerfile for the image `nxie/aio-miner`
I based it off the ethminer Dockerfile, updating CUDA to 11 and adding the different miners.

Here are some example arguments you can pass through vast
```bash
nbminer/nbminer -d 0 -a kawpow -o stratum+tcp://kawpow.usa.nicehash.com:3385 -u youraddress.9:d=3072
```

```bash
claymore/ethdcrminer64 <see_miner_docs>
```

```bash
xmrig/xmrig <see_miner_docs>
```

```bash
phoenixminer/PhoenixMiner <see_miner_docs>
```
```bash
ethminer/ethminer <see_miner_docs>
```

## Ideas

Some things I'd like to make when I have time

- Idle time logger. View least active days etc.
- Wallet based authentication on gpu-profile
- Simple mining profitability switcher
- Bid watcher. Watch for GPUs that reach a certain price per hour and rent them automatically
