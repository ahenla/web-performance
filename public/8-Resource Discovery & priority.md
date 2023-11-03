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

bf cache -> back / forward cache
