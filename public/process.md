www.somesite.com

process:

1-DNS query - 100ms

2-TCP connection - 120ms

3-SSL Negotiation - 150ms

4-HTTP request - uplink
Header - Body

5-Server process (backend-time) - 200ms to 500ms

6-HTTP response - downlink
Header - Body

7-Browsers HTML parsing

8-Resource Discovery & priority

Resource Discovery queue:
-cache headers per file
--Absolute expiration date
--Relative expiration date
--More specs / values

Browser needs a resource:
-It checks the cache
--cache MISS -> go to the network
--cache HIT
---it's expired
----conditional request -> not modified (update cache expiration date) or modified (new file)
---its not expired
----use the file from the cache

9-Render (layout, paint)

LCP - budget 2.5s limit
