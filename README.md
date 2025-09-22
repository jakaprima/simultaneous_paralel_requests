# Load Test with hey

## HOW TO USE

### Install
```bash
go install github.com/rakyll/hey@latest

# Check already installed
which hey

# RUN
# 🔹 -n 10 = total 10 request
# 🔹 -c 10 = semua 10 request dikirim simultaneously (bareng)
cat payloads.txt | head -n 5 | xargs -I{} -P5 ~/go/bin/hey -n 10 -c 10 \
  -m POST \
  -H "Content-Type: application/json" \
  -d '{}' \
  https://reqres.in/api/users

# Example Output
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

Latency distribution:
  0% in 0.0000 secs

Details (average, fastest, slowest):
  DNS+dialup:	1.2709 secs, 1.4754 secs, 1.4754 secs
  DNS-lookup:	1.2311 secs, 1.2311 secs, 1.2311 secs
  req write:	0.0003 secs, 0.0003 secs, 0.0003 secs
  resp wait:	0.2039 secs, 0.2039 secs, 0.2039 secs
  resp read:	0.0003 secs, 0.0003 secs, 0.0003 secs

Status code distribution:
  [400]	1 responses


# simultant with different headers and payload
# path ke hey (ganti ~/go/bin/hey kalau butuh)
HEY=~/go/bin/hey

cat header_payloads.txt | xargs -I{} -P5 sh -c '
  line="{}"
  header=$(printf "%s" "$line" | awk -F"||" "{print \$1}")
  body=$(printf "%s" "$line" | awk -F"||" "{print \$2}")
  '"$HEY"' -n 1 -c 1 -m POST -H "$header" -H "Content-Type: application/json" -d "$body" https://reqres.in/api/users
'
```