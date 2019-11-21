# Admission Webhooks: Configuration and Debugging Best Practices - Haowei Cai, Google
- Best practices:
  - Idempotence
     - Ordering is hard
     - Reinvocation of the web-hooks (best effort) does call the web hooks twice
  - Intercepting all versions of an object
     - v1beta1
     - v1beta2
     - etc
  - Availability 
     - timeoutseconds is recommended to 2
  - good to have a validating web hooks
      - example with the always pull and side car web hook.
  - Avoid working on the kube-system namespace (use namespace selector)


  # Liberating K8s From Kube Proxy And Iptables
  - /boot/config is not set with NETFILTER
  - kube-proxy resets the iptables periodically

# Mitigating Noisy Neighbours: Advanced Container Resource Management - Alexander Kanevskiy, Intel
 - rsrcctrl
 - OCI spec
    • blkio: IOPS / bps throttling
    • HugePages
    • Intel® RDT class
    • Hooks {we can have additional exec hooks with OCI specs.. checkout the pr#1008}


# Debugging Live Applications In Kubernetes
  - 