# Pod Controllor (for Application)

###### tags: `K8s` `kubernetes` 

`Kubernetes` 裡最基礎的運算單位是 `pod`，而 `pod` 可由 `controllor` 控制。以 `Docker` 角度來說 `pod` 像是使用指令 `docker run` 所啟動的程序，而 `controllor` 就像是由 `docker-compose` 啟動的；實際上 `docker-compose` 比本篇要提的 `Controllor` 要來的複雜許多。

`Kubernetes` 所提供的 `Controllor` 依用途，我會先將其區分為以下兩大類

* Job Controllor
    
  `CronJob`、`Job`
  
* Application Controllor

  `Deployment`、`DaemonSet`、`StatefulSet`、

本篇主題，主要在說明 `Application Controllor` 的用途 

---

## Deployment

`Deployment` 最適合用於部署無狀態類的應用，如擴充分流。kubernetes.io `Controllor` 篇，還有兩個類似功能 `ReplicaSet` & `ReplicationController`，這兩個功能與 `Deployment` 完全重疊，完全不需閱讀，官方建議一律改用 `Deployment`

> Note: A Deployment that configures a ReplicaSet is now the recommended way to set up replication.

