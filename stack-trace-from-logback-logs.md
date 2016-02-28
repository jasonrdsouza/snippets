# Extract and Pretty Print Stack Trace from Logback Logs

```bash
cat tmp | jq ".stack_trace" | xargs printf
```
