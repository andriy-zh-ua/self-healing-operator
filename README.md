# self-healing-operator

## Features

The self-healing operator monitors deployments and automatically responds to common issues:

### Monitored Conditions
- **Too many restarts**: Detects when pods are restarting frequently
- **High memory usage**: Identifies memory pressure and resource exhaustion
- **Failing health probes**: Responds to failed liveness and readiness probes
- **Unhealthy pods**: Detects pods in failed or pending states 

### Automatic Actions
- **Restart pods**: Automatically restart problematic pods
- **Scale replicas**: Adjust replica count based on conditions
- **Recreate deployment**: Force recreation of the entire deployment when needed
- **Notify Slack/webhook**: Send alerts to external monitoring systems

## Usage

The operator continuously watches deployments in the cluster and applies healing policies based on configurable thresholds and rules.
