---
layout: post
title:  "Expired SSL certificates"
date:   2021-06-08 14:00:00 +0100
categories: server
---

Due to a unnoticed Python compatibility-issue on a central services, we
were unable to renew certificates for a prolonged period of time.

This caused the certificates on all servers to expire without getting renewed.

If you were using a client which does certificate-validation, this would cause the server to be
unavailable, unless you explicitly disabled validation.

This issue is now resolved, and servers should be able to update their certificatates again.

Sorry about the inconvenience.
