# Query.AI-kibana-plugin

## Install
`./bin/kibana-plugin install https://github.com/sunminxuan/Query.AI-kibana-plugin/releases/download/7.2.0/query_ai-7.2.0.zip`

Add below lines in kibana.yml
```
csp.rules:
  # current defaults
  - "script-src 'unsafe-eval' 'nonce-{nonce}'"
  - "worker-src blob'"
  - "child-src blob:"
  # New rule for iframes
  - "frame-src https://ai.query.ai/"
 ```