# MTA-STS policy for thearknewspaper.com

Serves `https://mta-sts.thearknewspaper.com/.well-known/mta-sts.txt`, which tells other mail servers to deliver mail to The Ark only over verified TLS to Google's MX hosts.

Mode starts as `testing` (report only). After ~2 weeks of clean TLS-RPT reports, change `mode:` to `enforce`, then bump the `id=` in the `_mta-sts` DNS TXT record.
