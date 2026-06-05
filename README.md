# Welcome to Solsgate

This is a repo for new users getting started with Docker.

## Gulefirdous MVP

The current Gulefirdous work adds:

- A React MVP dashboard for product drafts, Facebook/Instagram publishing actions,
  COD ordering, TCS tracking, referrals, and source analytics.
- A Node backend proxy under `backend/` for secure WooCommerce product/order sync.

WordPress status checked on `gulefirdous.com`:

- WooCommerce is installed and active.
- Cash on Delivery is enabled.
- Store country/currency are still set to United States/USD and should only be
  changed after confirming the correct base country and currency.

Do not place WooCommerce API secrets in the frontend. Store them in backend
environment variables using `backend/.env.example` as the template.

You can try it out using the following command.
```
docker run -d -p 8080:80 --name webserver solsgate
```
And open `http://localhost:8080` in your browser.

# Building

Maintainers should see [MAINTAINERS.md](MAINTAINERS.md).

Build and run:
```
docker build -t solsgate . 
docker run -d -p 8080:3000 --name webserver solsgate
```
Open `http://localhost:8080` in your browser.
