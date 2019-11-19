# Admission Webhooks: Configuration and Debugging Best Practices - Haowei Cai, Google
- Best practices:
  - Idempotence
     - Ordering is hard
     - Reinvocation of the web-hooks (best effort) does call the web hooks twice
  - Intercepting all versions of an object
     - v1beta1
     - v1beta2
     - etc