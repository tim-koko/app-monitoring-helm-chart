# Monitoring

This Repo contains the source to the monitoring helm chart. The helm chart provides funtionality to deploy and manage monitoring capabilities for the financial-data-hub application containing the following components:

- AlertmanagerConfig
- general Prometheus (https://github.com/kubernetes-monitoring/kubernetes-mixin)
  - kubernetes-apps
    - KubePodCrashLooping
    - KubePodNotReady
    - KubeDeploymentGenerationMismatch
    - KubeDeploymentReplicasMismatch
    - KubeDeploymentRolloutStuck
    - KubeStatefulSetReplicasMismatch
    - KubeStatefulSetGenerationMismatch
    - KubeStatefulSetUpdateNotRolledOut
    - KubeDaemonSetRolloutStuck
    - KubeContainerWaiting
    - KubeDaemonSetNotScheduled
    - KubeDaemonSetMisScheduled
    - KubeJobNotCompleted
    - KubeJobFailed
    - KubeHpaReplicasMismatch
    - KubeHpaMaxedOut
  - kubernetes-resources
    - KubeCPUQuotaOvercommit
    - KubeMemoryQuotaOvercommit
    - KubeQuotaAlmostFull
    - KubeQuotaFullyUsed
    - KubeQuotaExceeded
    - KubePersistentVolumeFillingUp (warning: based on last 6h will be full in 4d, critical: 90% full)
    - KubePersistentVolumeInodesFillingUp (warning: based on last 6h will be full in 4d, critical: 90% full)
    - KubePersistentVolumeErrors
  - kubernetes-general-application
    - ThrottledContainers
    - KubePodRestarting
    - KubeDeploymentReplicasNotReady

## License

This project is licensed under the **Apache 2.0 License**. See the [LICENSE](LICENSE) file for details.
