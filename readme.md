# Saif Abdelrazek || DNS

## Description

This is a dns service for my domain names. It is a simple service that allows me and any one to add, remove and list dns records for the provided domain names.

This service is using [OctoDNS](https://github.com/octodns/octodns) for managing the dns records through yaml files. It is also connected to [Cloudflare](https://www.cloudflare.com/) for hosting the dns records.

### Currently provided domains:

- saifabdelrazek.com

Working for adding more in the upcoming future.

### How to use it

1. Fork the repo.
2. Add a subdomain to any of the YAML files in the `zones` folder like this:

   ```yaml
   example:
     ttl: 600
     type: CNAME
     value: cname.vercel-dns.com.
   ```

3. Create a pull request to the main branch of the repo.
4. The pull request will be reviewed and merged if it is valid.
5. The DNS records will be updated automatically using GitHub Actions.
