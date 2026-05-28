# Pi-hole Blocklist

Custom Pi-hole blocklist for ads, telemetry, tracking, and unwanted domains.

## Features

* Ad blocking
* Telemetry blocking
* Gaming tracker blocking
* Microsoft tracking reduction
* Easy integration with Pi-hole

## Repository Structure

```text
hosts/
├── ads.txt
├── telemetry.txt
├── malware.txt
└── gaming.txt
```

## Usage

Add raw list URLs to Pi-hole:

```text
Group Management > Adlists
```

Example:

```text
https://raw.githubusercontent.com/<yourusername>/pihole-blocklists/main/hosts/ads.txt
```

## Update Gravity

Run:

```bash
pihole -g
```

## Recommended Format

Each file should contain one domain per line.

Example:

```text
ads.example.com
tracker.example.net
telemetry.example.org
```

## Goals

* Keep lists clean
* Avoid false positives
* Separate categories logically
* Maintain easy auditing

## License

MIT License
