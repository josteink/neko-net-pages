---
layout: post
title:  "Expired SSL certificates"
date:   2018-07-39 11:00:00 +0100
categories: server
---

Due to an incomplete DNS-migration from GoDaddy to Cloudflare, all servers in the network
were unable to retrieve updated certificates.

This caused Oslo (and possibly other servers) to fail to update the certificates in time
before expiration.

If you're using a client which does certificate-validation, this would cause the server to be
unavailable, unless you explicitly disabled validation.

This issue is now resolved, and servers should be able to update their certificatates again.

Sorry about the inconvenience.
