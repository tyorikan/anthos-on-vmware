## Default installed systems

```
ubuntu@gke-admin-ws-210517-022057:~$ k get all -A --kubeconfig vmw-user-cluster-kubeconfig
NAMESPACE                 NAME                                                           READY   STATUS    RESTARTS   AGE
anthos-identity-service   pod/ais-69858bdd6c-xn474                                       1/1     Running   0          55m
gke-connect               pod/gke-connect-agent-20210129-01-00-59c9dc4b4-98nfl           1/1     Running   0          50m
gke-system                pod/istio-ingress-65cfb6b7df-8gdb5                             2/2     Running   0          55m
gke-system                pod/istio-ingress-65cfb6b7df-rrv8j                             2/2     Running   0          55m
gke-system                pod/istio-pilot-56f545d6f5-2xqmf                               1/1     Running   0          55m
gke-system                pod/istio-pilot-56f545d6f5-hvcdd                               1/1     Running   0          55m
kube-system               pod/anthos-metering-5bfd6c97cc-b6sqk                           1/1     Running   0          55m
kube-system               pod/anthos-metering-5bfd6c97cc-lh45w                           1/1     Running   0          55m
kube-system               pod/anthos-metering-5bfd6c97cc-zj59d                           1/1     Running   0          55m
kube-system               pod/calico-node-855wc                                          1/1     Running   0          53m
kube-system               pod/calico-node-dc4bj                                          1/1     Running   0          53m
kube-system               pod/calico-node-dqk27                                          1/1     Running   0          53m
kube-system               pod/calico-typha-86ccc496-v7bkw                                1/1     Running   0          52m
kube-system               pod/calico-typha-86ccc496-vjh5w                                1/1     Running   0          55m
kube-system               pod/calico-typha-horizontal-autoscaler-5bbb889d55-x8mzw        1/1     Running   0          55m
kube-system               pod/citadel-57ffb4d76-lgv92                                    1/1     Running   0          54m
kube-system               pod/clientconfig-operator-54d9d45999-tk2l9                     1/1     Running   0          55m
kube-system               pod/csi-snapshot-validation-6f69b896d4-4vrk5                   1/1     Running   0          55m
kube-system               pod/kube-dns-54cbf97d6f-kcspm                                  3/3     Running   0          55m
kube-system               pod/kube-dns-54cbf97d6f-v8khd                                  3/3     Running   0          55m
kube-system               pod/kube-dns-autoscaler-58b965c566-w4hgd                       1/1     Running   0          55m
kube-system               pod/kube-proxy-82lqk                                           1/1     Running   0          53m
kube-system               pod/kube-proxy-crj99                                           1/1     Running   0          53m
kube-system               pod/kube-proxy-lg8wb                                           1/1     Running   0          53m
kube-system               pod/kube-state-metrics-5bd467c845-9scwc                        3/3     Running   0          51m
kube-system               pod/load-balancer-seesaw-84b8fbc764-bxlbc                      2/2     Running   0          55m
kube-system               pod/metrics-server-5f57b546db-p4tc4                            2/2     Running   0          51m
kube-system               pod/node-exporter-6kt9p                                        2/2     Running   0          53m
kube-system               pod/node-exporter-77pp5                                        2/2     Running   0          53m
kube-system               pod/node-exporter-d2g5f                                        2/2     Running   0          53m
kube-system               pod/stackdriver-log-forwarder-4qbbr                            1/1     Running   0          52m
kube-system               pod/stackdriver-log-forwarder-t6jrq                            1/1     Running   0          52m
kube-system               pod/stackdriver-log-forwarder-zs68j                            1/1     Running   0          52m
kube-system               pod/stackdriver-metadata-agent-cluster-level-877ff55f6-mcldm   1/1     Running   0          52m
kube-system               pod/stackdriver-operator-6478d955dc-85zrh                      2/2     Running   0          55m
kube-system               pod/stackdriver-prometheus-k8s-0                               2/2     Running   0          52m

NAMESPACE                 NAME                                               TYPE           CLUSTER-IP     EXTERNAL-IP   PORT(S)                                 AGE
anthos-identity-service   service/ais                                        ClusterIP      10.96.10.182   <none>        443/TCP,9901/TCP                        56m
default                   service/kubernetes                                 ClusterIP      10.96.0.1      <none>        443/TCP                                 56m
gke-connect               service/gke-connect-monitoring                     ClusterIP      10.96.2.43     <none>        8080/TCP                                50m
gke-system                service/istio-ingress                              LoadBalancer   10.96.0.57     10.0.10.202   80:32025/TCP,443:32120/TCP              55m
gke-system                service/istio-pilot                                ClusterIP      10.96.13.124   <none>        15010/TCP,15011/TCP,8080/TCP,9093/TCP   55m
kube-system               service/alertmanager-operated                      ClusterIP      None           <none>        6783/TCP,9443/TCP                       54m
kube-system               service/calico-typha                               ClusterIP      10.96.14.203   <none>        5473/TCP                                56m
kube-system               service/clientconfig-operator                      ClusterIP      10.96.11.91    <none>        443/TCP                                 56m
kube-system               service/csi-snapshot-validation-service            ClusterIP      10.96.9.166    <none>        23011/TCP                               55m
kube-system               service/kube-dns                                   ClusterIP      10.96.0.10     <none>        53/UDP,53/TCP                           56m
kube-system               service/kube-state-metrics                         ClusterIP      10.96.7.15     <none>        9443/TCP                                54m
kube-system               service/metrics-server                             ClusterIP      10.96.10.76    <none>        443/TCP                                 55m
kube-system               service/seesaw-for-vmw-user-cluster-pljnqh9zkh-1   ClusterIP      None           <none>        20257/TCP                               56m
kube-system               service/stackdriver-operator                       ClusterIP      10.96.8.227    <none>        9090/TCP                                55m
kube-system               service/stackdriver-prometheus-k8s                 ClusterIP      None           <none>        9090/TCP                                52m

NAMESPACE     NAME                                       DESIRED   CURRENT   READY   UP-TO-DATE   AVAILABLE   NODE SELECTOR            AGE
kube-system   daemonset.apps/calico-node                 3         3         3       3            3           kubernetes.io/os=linux   56m
kube-system   daemonset.apps/kube-proxy                  3         3         3       3            3           kubernetes.io/os=linux   55m
kube-system   daemonset.apps/node-exporter               3         3         3       3            3           kubernetes.io/os=linux   54m
kube-system   daemonset.apps/stackdriver-log-forwarder   3         3         3       3            3           kubernetes.io/os=linux   52m

NAMESPACE                 NAME                                                       READY   UP-TO-DATE   AVAILABLE   AGE
anthos-identity-service   deployment.apps/ais                                        1/1     1            1           56m
gke-connect               deployment.apps/gke-connect-agent-20210129-01-00           1/1     1            1           50m
gke-system                deployment.apps/istio-ingress                              2/2     2            2           55m
gke-system                deployment.apps/istio-pilot                                2/2     2            2           55m
kube-system               deployment.apps/anthos-metering                            3/3     3            3           56m
kube-system               deployment.apps/calico-typha                               2/2     2            2           56m
kube-system               deployment.apps/calico-typha-horizontal-autoscaler         1/1     1            1           55m
kube-system               deployment.apps/citadel                                    1/1     1            1           54m
kube-system               deployment.apps/clientconfig-operator                      1/1     1            1           56m
kube-system               deployment.apps/csi-snapshot-validation                    1/1     1            1           55m
kube-system               deployment.apps/kube-dns                                   2/2     2            2           56m
kube-system               deployment.apps/kube-dns-autoscaler                        1/1     1            1           56m
kube-system               deployment.apps/kube-state-metrics                         1/1     1            1           54m
kube-system               deployment.apps/load-balancer-seesaw                       1/1     1            1           56m
kube-system               deployment.apps/metrics-server                             1/1     1            1           55m
kube-system               deployment.apps/stackdriver-metadata-agent-cluster-level   1/1     1            1           52m
kube-system               deployment.apps/stackdriver-operator                       1/1     1            1           55m

NAMESPACE                 NAME                                                                 DESIRED   CURRENT   READY   AGE
anthos-identity-service   replicaset.apps/ais-69858bdd6c                                       1         1         1       55m
gke-connect               replicaset.apps/gke-connect-agent-20210129-01-00-59c9dc4b4           1         1         1       50m
gke-system                replicaset.apps/istio-ingress-65cfb6b7df                             2         2         2       55m
gke-system                replicaset.apps/istio-pilot-56f545d6f5                               2         2         2       55m
kube-system               replicaset.apps/anthos-metering-5bfd6c97cc                           3         3         3       55m
kube-system               replicaset.apps/calico-typha-86ccc496                                2         2         2       55m
kube-system               replicaset.apps/calico-typha-horizontal-autoscaler-5bbb889d55        1         1         1       55m
kube-system               replicaset.apps/citadel-57ffb4d76                                    1         1         1       54m
kube-system               replicaset.apps/clientconfig-operator-54d9d45999                     1         1         1       55m
kube-system               replicaset.apps/csi-snapshot-validation-6f69b896d4                   1         1         1       55m
kube-system               replicaset.apps/kube-dns-54cbf97d6f                                  2         2         2       55m
kube-system               replicaset.apps/kube-dns-autoscaler-58b965c566                       1         1         1       55m
kube-system               replicaset.apps/kube-state-metrics-5bd467c845                        1         1         1       51m
kube-system               replicaset.apps/kube-state-metrics-9c6857d67                         0         0         0       54m
kube-system               replicaset.apps/load-balancer-seesaw-84b8fbc764                      1         1         1       55m
kube-system               replicaset.apps/metrics-server-5f57b546db                            1         1         1       51m
kube-system               replicaset.apps/metrics-server-986848cd6                             0         0         0       55m
kube-system               replicaset.apps/stackdriver-metadata-agent-cluster-level-877ff55f6   1         1         1       52m
kube-system               replicaset.apps/stackdriver-operator-6478d955dc                      1         1         1       55m

NAMESPACE     NAME                                          READY   AGE
kube-system   statefulset.apps/stackdriver-prometheus-k8s   1/1     52m

NAMESPACE    NAME                                                    REFERENCE                  TARGETS   MINPODS   MAXPODS   REPLICAS   AGE
gke-system   horizontalpodautoscaler.autoscaling/istio-ingress-hpa   Deployment/istio-ingress   2%/80%    2         5         2          55m
gke-system   horizontalpodautoscaler.autoscaling/istio-pilot-hpa     Deployment/istio-pilot     2%/80%    2         5         2          55m
```

## CRDs
```
ubuntu@gke-admin-ws-210517-022057:~$ k get crds -A --kubeconfig vmw-user-cluster-kubeconfig
NAME                                                         CREATED AT
applications.app.k8s.io                                      2021-05-18T06:30:48Z
authorizationpolicies.security.istio.io                      2021-05-18T06:33:59Z
bgpconfigurations.crd.projectcalico.org                      2021-05-18T06:30:54Z
bgppeers.crd.projectcalico.org                               2021-05-18T06:30:54Z
blockaffinities.crd.projectcalico.org                        2021-05-18T06:30:57Z
clientconfigs.authentication.gke.io                          2021-05-18T06:30:48Z
clusterinformations.crd.projectcalico.org                    2021-05-18T06:30:55Z
clusterrbacconfigs.rbac.istio.io                             2021-05-18T06:33:59Z
clusters.cluster.k8s.io                                      2021-05-18T06:30:46Z
destinationrules.networking.istio.io                         2021-05-18T06:33:59Z
entitlements.anthos.gke.io                                   2021-05-18T06:36:39Z
envoyfilters.networking.istio.io                             2021-05-18T06:33:59Z
felixconfigurations.crd.projectcalico.org                    2021-05-18T06:30:54Z
gateways.networking.istio.io                                 2021-05-18T06:30:59Z
globalnetworkpolicies.crd.projectcalico.org                  2021-05-18T06:30:55Z
globalnetworksets.crd.projectcalico.org                      2021-05-18T06:30:55Z
hostendpoints.crd.projectcalico.org                          2021-05-18T06:30:54Z
httpapispecbindings.config.istio.io                          2021-05-18T06:33:59Z
httpapispecs.config.istio.io                                 2021-05-18T06:33:59Z
ipamblocks.crd.projectcalico.org                             2021-05-18T06:30:57Z
ipamconfigs.crd.projectcalico.org                            2021-05-18T06:30:58Z
ipamhandles.crd.projectcalico.org                            2021-05-18T06:30:57Z
ippools.crd.projectcalico.org                                2021-05-18T06:30:54Z
machineclasses.cluster.k8s.io                                2021-05-18T06:30:46Z
machinedeployments.cluster.k8s.io                            2021-05-18T06:30:46Z
machines.cluster.k8s.io                                      2021-05-18T06:30:46Z
machinesets.cluster.k8s.io                                   2021-05-18T06:30:46Z
memberships.hub.gke.io                                       2021-05-18T06:36:13Z
meshpolicies.authentication.istio.io                         2021-05-18T06:33:59Z
metricsserver.addons.k8s.io                                  2021-05-18T06:31:05Z
monitoring.addons.k8s.io                                     2021-05-18T06:31:00Z
networkpolicies.crd.projectcalico.org                        2021-05-18T06:30:56Z
networksets.crd.projectcalico.org                            2021-05-18T06:30:56Z
onpremnodepools.onprem.cluster.gke.io                        2021-05-18T06:30:47Z
onpremuserclusters.onprem.cluster.gke.io                     2021-05-18T06:30:47Z
policies.authentication.istio.io                             2021-05-18T06:33:59Z
quotaspecbindings.config.istio.io                            2021-05-18T06:33:59Z
quotaspecs.config.istio.io                                   2021-05-18T06:33:59Z
rbacconfigs.rbac.istio.io                                    2021-05-18T06:33:59Z
seesawgroups.seesaw.gke.io                                   2021-05-18T06:30:48Z
serviceentries.networking.istio.io                           2021-05-18T06:33:59Z
servicerolebindings.rbac.istio.io                            2021-05-18T06:33:59Z
serviceroles.rbac.istio.io                                   2021-05-18T06:33:59Z
sidecars.networking.istio.io                                 2021-05-18T06:33:59Z
stackdrivers.addons.sigs.k8s.io                              2021-05-18T06:31:08Z
syntheticserviceentries.networking.istio.io                  2021-05-18T06:33:59Z
usagerecords.metering.gke.io                                 2021-05-18T06:30:48Z
virtualservices.networking.istio.io                          2021-05-18T06:33:59Z
volumesnapshotclasses.snapshot.storage.k8s.io                2021-05-18T06:30:58Z
volumesnapshotcontents.snapshot.storage.k8s.io               2021-05-18T06:30:59Z
volumesnapshots.snapshot.storage.k8s.io                      2021-05-18T06:30:59Z
vsphereclusterproviderconfigs.vsphereproviderconfig.k8s.io   2021-05-18T06:30:46Z
vspheremachineproviderconfigs.vsphereproviderconfig.k8s.io   2021-05-18T06:30:46Z
```