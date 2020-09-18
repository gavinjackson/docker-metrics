# docker-metrics
A small sample project that harvests and presents docker (and host) metrics via grafana.

The *docker-compose.yml* file defines the following four containers:

1. *cadvisor* collects container stats
2. *node-exporter* collects physical hardware stats.
3. *prometheus* harvests this data.
4. *grafana* is provisioned to consume data from the prometheus server and present some pre-made dashboards to visualise the data.

The cool thing about this is that you can copy this into your existing docker project and you will get instant metrics for all of your running containers (and host system).

# How to run
1. docker-compose up
2. Sign in to http://localhost:3000 (admin/password)
