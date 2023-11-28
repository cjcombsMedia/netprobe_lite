# Netprobe Lite

Simple and effective tool for measuring ISP performance at home. The tool measures several performance metrics including packet loss, latency and DNS performance. It also aggregates these metrics into a common score, which you can use to monitor overall health of your internet connection.

## Requirements and Setup

To run Netprobe Lite, you'll need a PC running Docker connected directly to your ISP router. Specificially:

1. Netprobe Lite requires the latest version of Docker. For instructions on installing Docker, see YouTube, it's super easy.

2. Netprobe Lite should be installed on a machine (the 'probe') which has a wired Ethernet connectiont to your primary ISP router. This ensures the tests are accurately measuring your ISP performance and excluding and interference from your home network. An old PC with Linux installed is a great option for this.

# Installation

1. Clone the repo locally to the probe machine:

```
git clone https://github.com/riyaadali/netprobe_lite.git
```

2. From the cloned folder, using docker compose to launch the app:

```
docker compose up
```

# How to use

1. Navigate to: http://x.x.x.x:3001/ where x.x.x.x = IP of the probe machine running Docker.

2. Default user / pass is 'admin/admin'. Login to Grafana and set a custom password.

3. Click on 'Menu -> Dashboards -> Netprobe' to view the dashboard (you should add the URL as a bookmark).
