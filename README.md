# docker-local-lemp
Local LEMP stack for development. Also includes phpMyAdmin for easier database development/debugging.

## Instructions/Usage:
1. Clone and run `docker-compose build` then `docker-compose up`
2. You will then have the contents of the public folder served on http://localhost:8080
3. phpMyAdmin can be accessed from http://localhost:8181 (use credentials for root from docker-compose, and database name is 'mysql')

### Note: Shoutout to phpdocker.io for a great online tool that helped form a starting point for this configuration.
