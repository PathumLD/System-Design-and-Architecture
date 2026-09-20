# Lesson 42 --- Kubernetes Networking and Storage

## Networking

``` text
Pod
 ↓
Service
 ↓
Ingress / Gateway
```

Kubernetes provides service discovery and cluster networking through its
networking stack.

## Security

NetworkPolicy can restrict pod-to-pod traffic.

## Storage

-   PersistentVolume
-   PersistentVolumeClaim
-   StorageClass

Persistent storage is different from backup.

For cloud-native applications, object storage such as Azure Blob is
often preferable to shared filesystem storage for user files.
