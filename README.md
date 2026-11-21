<p align="center">
    <picture>
        <source media="(prefers-color-scheme: dark)" srcset="https://cdn.karlosoft.com/cdn-data/ks/img/kprobe/logo.svg">
        <source media="(prefers-color-scheme: light)" srcset="https://cdn.karlosoft.com/cdn-data/ks/img/kprobe/logo-dark.svg">
        <img alt="Enplated Email" src="https://cdn.karlosoft.com/cdn-data/ks/img/kprobe/logo-dark.svg" width="700">
    </picture>
    <br>
    <strong>Lightweight self-hosted probe for monitoring devices in your local network.</strong>
    <br>
    <br>
    <br>
    <br>
    <img src="https://cdn.karlosoft.com/cdn-data/ks/img/kprobe/github.png" width="700" alt="K-Probe">
</p>


## What is K-Probe?
- **K-Probe is a lightweight, standalone monitoring system designed to run locally inside your network.**
- It actively checks local devices – such as Wi-Fi access points, IP cameras, printers, and internal servers – using ping (ICMP) and HTTP requests.
- The status of these checks is exposed through a clean **HTTP API**, allowing you to easily integrate it with external monitoring dashboards like Uptime Kuma, Zabbix, or any custom tool of your choice.
- It is designed to be self-contained, easy to deploy, and runs completely independently on your local machine or server.

<br>

## How Does It Work?
1. **Deploy**: Set up a small local server or VM running Linux (Ubuntu, Debian, CentOS, RHEL, Rocky Linux, or Fedora).
2. **Install**: Install K-Probe using our native `.deb` or `.rpm` packages as detailed in [FAQ.md](FAQ.md).
3. **Configure**: Define the local devices and services you want to monitor.
4. **Integrate**: Point your favorite monitoring system (e.g., Uptime Kuma) to the K-Probe API endpoint. 
   - The API provides straightforward JSON responses showing the status of each scan, allowing you to monitor internal networks securely without exposing them directly to the internet.

<br>

## Features
- **ICMP Ping Checks**: Monitor device availability with customizable timeouts and retry counts.
- **HTTP/HTTPS Scans**: Check web interfaces with timeout limits, expected HTTP status codes, and advanced response validation.
- **Dynamic Expression Engine**: Extract and evaluate variables from HTTP responses using JSON paths, boolean keywords, and logical operators (`&&`, `||`, `!`, comparisons).
- **Simple Web Editor & CLI**: A minimal web-based configuration editor and a full-featured CLI to manage everything easily.
- **Standalone API Server**: A dedicated, lightweight API service to fetch scan results on demand.

<br>

## Can I Use It Without Uptime Kuma?
- Absolutely. The HTTP API is fully standalone, meaning you can query scan statuses directly, integrate them into your own dashboards, or write simple scripts to process the results.

- Please note:
    - K-Probe is focused entirely on local execution and state reporting; it does **not** send notifications.
    - There are no plans to add alerting features, as it is intended to feed status data to systems that already handle notifications.

<br>

## Getting Started
- For complete installation guides, command references, and troubleshooting, check out [FAQ.md](FAQ.md).

<br>
<br>

---

#### K-Probe is an independent open-source project developed by Karel Cermak (info@karlosoft.com). It is not affiliated with Uptime Kuma, Zabbix, or any other monitoring platform.
