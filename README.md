HOW TO USE:
install:
go install github.com/rakyll/hey@latest

check already installed:
which hey

RUN:
cat payloads.txt | head -n 5 | xargs -I{} -P5 ~/go/bin/hey -n 1 -c 1 \
  -m POST \
  -H "Content-Type: application/json" \
  -d '{}' \
  https://reqres.in/api/users




RESULTS:
Summary:
  Total:	1.4755 secs
  Slowest:	1.4754 secs
  Fastest:	1.4754 secs
  Average:	1.4754 secs
  Requests/sec:	0.6777
  
  Total data:	338 bytes
  Size/request:	338 bytes

Response time histogram:
  1.475 [1]	|■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■
  1.475 [0]	|
  1.475 [0]	|
  1.475 [0]	|
  1.475 [0]	|
  1.475 [0]	|
  1.475 [0]	|
  1.475 [0]	|
  1.475 [0]	|
  1.475 [0]	|
  1.475 [0]	|


Latency distribution:
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs

Details (average, fastest, slowest):
  DNS+dialup:	1.2709 secs, 1.4754 secs, 1.4754 secs
  DNS-lookup:	1.2311 secs, 1.2311 secs, 1.2311 secs
  req write:	0.0003 secs, 0.0003 secs, 0.0003 secs
  resp wait:	0.2039 secs, 0.2039 secs, 0.2039 secs
  resp read:	0.0003 secs, 0.0003 secs, 0.0003 secs

Status code distribution:
  [400]	1 responses




Summary:
  Total:	1.4758 secs
  Slowest:	1.4758 secs
  Fastest:	1.4758 secs
  Average:	1.4758 secs
  Requests/sec:	0.6776
  
  Total data:	338 bytes
  Size/request:	338 bytes

Response time histogram:
  1.476 [1]	|■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■
  1.476 [0]	|
  1.476 [0]	|
  1.476 [0]	|
  1.476 [0]	|
  1.476 [0]	|
  1.476 [0]	|
  1.476 [0]	|
  1.476 [0]	|
  1.476 [0]	|
  1.476 [0]	|


Latency distribution:
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs

Details (average, fastest, slowest):
  DNS+dialup:	1.2717 secs, 1.4758 secs, 1.4758 secs
  DNS-lookup:	1.2290 secs, 1.2290 secs, 1.2290 secs
  req write:	0.0001 secs, 0.0001 secs, 0.0001 secs
  resp wait:	0.2035 secs, 0.2035 secs, 0.2035 secs
  resp read:	0.0003 secs, 0.0003 secs, 0.0003 secs

Status code distribution:
  [400]	1 responses




Summary:
  Total:	1.4914 secs
  Slowest:	1.4914 secs
  Fastest:	1.4914 secs
  Average:	1.4914 secs
  Requests/sec:	0.6705
  
  Total data:	338 bytes
  Size/request:	338 bytes

Response time histogram:
  1.491 [1]	|■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■
  1.491 [0]	|
  1.491 [0]	|
  1.491 [0]	|
  1.491 [0]	|
  1.491 [0]	|
  1.491 [0]	|
  1.491 [0]	|
  1.491 [0]	|
  1.491 [0]	|
  1.491 [0]	|


Latency distribution:
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs

Details (average, fastest, slowest):
  DNS+dialup:	1.2720 secs, 1.4914 secs, 1.4914 secs
  DNS-lookup:	1.2297 secs, 1.2297 secs, 1.2297 secs
  req write:	0.0002 secs, 0.0002 secs, 0.0002 secs
  resp wait:	0.2189 secs, 0.2189 secs, 0.2189 secs
  resp read:	0.0002 secs, 0.0002 secs, 0.0002 secs

Status code distribution:
  [400]	1 responses




Summary:
  Total:	1.5012 secs
  Slowest:	1.5012 secs
  Fastest:	1.5012 secs
  Average:	1.5012 secs
  Requests/sec:	0.6661
  
  Total data:	338 bytes
  Size/request:	338 bytes

Response time histogram:
  1.501 [1]	|■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■
  1.501 [0]	|
  1.501 [0]	|
  1.501 [0]	|
  1.501 [0]	|
  1.501 [0]	|
  1.501 [0]	|
  1.501 [0]	|
  1.501 [0]	|
  1.501 [0]	|
  1.501 [0]	|


Latency distribution:
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs

Details (average, fastest, slowest):
  DNS+dialup:	1.2730 secs, 1.5012 secs, 1.5012 secs
  DNS-lookup:	1.2302 secs, 1.2302 secs, 1.2302 secs
  req write:	0.0001 secs, 0.0001 secs, 0.0001 secs
  resp wait:	0.2276 secs, 0.2276 secs, 0.2276 secs
  resp read:	0.0003 secs, 0.0003 secs, 0.0003 secs

Status code distribution:
  [400]	1 responses




Summary:
  Total:	1.6720 secs
  Slowest:	1.6718 secs
  Fastest:	1.6718 secs
  Average:	1.6718 secs
  Requests/sec:	0.5981
  
  Total data:	338 bytes
  Size/request:	338 bytes

Response time histogram:
  1.672 [1]	|■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■
  1.672 [0]	|
  1.672 [0]	|
  1.672 [0]	|
  1.672 [0]	|
  1.672 [0]	|
  1.672 [0]	|
  1.672 [0]	|
  1.672 [0]	|
  1.672 [0]	|
  1.672 [0]	|


Latency distribution:
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs
  0% in 0.0000 secs

Details (average, fastest, slowest):
  DNS+dialup:	1.2715 secs, 1.6718 secs, 1.6718 secs
  DNS-lookup:	1.2283 secs, 1.2283 secs, 1.2283 secs
  req write:	0.0001 secs, 0.0001 secs, 0.0001 secs
  resp wait:	0.3998 secs, 0.3998 secs, 0.3998 secs
  resp read:	0.0002 secs, 0.0002 secs, 0.0002 secs

Status code distribution:
  [400]	1 responses


