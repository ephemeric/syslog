```
logger -T -n rocky9 -P 5516 slobwashere
```

```
for i in {1..10}; do builtin echo "my message" | logger -T -n 192.168.0.100 -P 5515; done
```

```
for i in {1..1000}; do logger -T -n 192.168.0.100 -P 5515 "$(cat log)"; done
```

```
for i in {1..10}; do logger -T -n 192.168.0.100 -P 7777 "$(cat log)"; done; tail -f fqdn
```

```
for i in {1..10}; do logger -T -n 192.168.0.100 -P 7777 "$(cat log)"; done; sleep 5; wc -l fqdn
```
