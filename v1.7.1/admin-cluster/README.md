## Default installed systems

```
ubuntu@gke-admin-ws-210517-022057:~$ kubectl get all -A --kubeconfig kubeconfig
NAMESPACE     NAME                                                            READY   STATUS    RESTARTS   AGE
kube-system   pod/calico-node-5kw9r                                           1/1     Running   0          8m4s
kube-system   pod/calico-node-cr4ps                                           1/1     Running   0          5m51s
kube-system   pod/calico-node-ftr5q                                           1/1     Running   0          5m49s
kube-system   pod/calico-typha-78fd7798bb-52pfk                               1/1     Running   0          8m4s
kube-system   pod/citadel-66dd66895b-cldrf                                    1/1     Running   0          4m48s
kube-system   pod/cluster-health-controller-79548b44b-lnd8w                   2/2     Running   0          4m46s
kube-system   pod/clusterapi-controllers-5cd6c9bb47-qs2rx                     3/3     Running   0          8m5s
kube-system   pod/etcd-admin-host1                                            1/1     Running   0          8m21s
kube-system   pod/gke-master-etcd-maintenance-7f4fff496b-2jhbb                1/1     Running   0          5m17s
kube-system   pod/kube-apiserver-admin-host1                                  1/1     Running   0          8m21s
kube-system   pod/kube-controller-manager-admin-host1                         1/1     Running   0          8m21s
kube-system   pod/kube-dns-5bdb9f84d-4qzqs                                    3/3     Running   0          8m5s
kube-system   pod/kube-dns-5bdb9f84d-6rkvs                                    3/3     Running   0          8m5s
kube-system   pod/kube-master-metrics-proxy-4wzbq                             1/1     Running   0          4m48s
kube-system   pod/kube-proxy-7wsmc                                            1/1     Running   0          5m51s
kube-system   pod/kube-proxy-9nqkw                                            1/1     Running   0          5m49s
kube-system   pod/kube-proxy-pv556                                            1/1     Running   0          8m
kube-system   pod/kube-scheduler-admin-host1                                  1/1     Running   0          8m21s
kube-system   pod/kube-state-metrics-69857cd5f6-khm6l                         3/3     Running   0          3m27s
kube-system   pod/load-balancer-seesaw-56c46ccf85-25j5k                       2/2     Running   0          7m59s
kube-system   pod/metrics-server-5f57b546db-x5skh                             2/2     Running   0          4m23s
kube-system   pod/metrics-server-operator-67d5c77897-vt8jl                    1/1     Running   0          4m55s
kube-system   pod/monitoring-operator-59d8d5f49c-h22lt                        1/1     Running   0          5m4s
kube-system   pod/node-exporter-88g9v                                         2/2     Running   0          4m48s
kube-system   pod/node-exporter-master-z6wcd                                  1/1     Running   0          4m48s
kube-system   pod/node-exporter-x9bjc                                         2/2     Running   0          4m48s
kube-system   pod/onprem-user-cluster-controller-784bbf9bff-6nkt9             2/2     Running   0          3m40s
kube-system   pod/pushprox-server-6f55784c5f-cnlr4                            2/2     Running   0          4m41s
kube-system   pod/stackdriver-log-forwarder-9rwk4                             1/1     Running   0          5m1s
kube-system   pod/stackdriver-log-forwarder-pm6c5                             1/1     Running   0          5m1s
kube-system   pod/stackdriver-log-forwarder-w94tj                             1/1     Running   0          5m1s
kube-system   pod/stackdriver-metadata-agent-cluster-level-7d59864ffb-7gdrw   1/1     Running   0          5m1s
kube-system   pod/stackdriver-operator-669b47ccfb-8rcp4                       2/2     Running   0          5m17s
kube-system   pod/stackdriver-prometheus-k8s-0                                2/2     Running   0          5m1s
kube-system   pod/vsphere-metrics-exporter-647db699f7-lkbqf                   2/2     Running   0          4m45s

NAMESPACE     NAME                                        TYPE           CLUSTER-IP      EXTERNAL-IP    PORT(S)             AGE
default       service/kubernetes                          ClusterIP      10.96.232.1     <none>         443/TCP             8m30s
kube-system   service/alertmanager-operated               ClusterIP      None            <none>         6783/TCP,9443/TCP   4m49s
kube-system   service/calico-typha                        ClusterIP      10.96.232.27    <none>         5473/TCP            8m5s
kube-system   service/cluster-health-controller           ClusterIP      10.96.232.241   <none>         9090/TCP            4m47s
kube-system   service/controller-manager                  ClusterIP      10.96.232.69    <none>         9090/TCP            8m6s
kube-system   service/external-pushprox-server            LoadBalancer   10.96.232.160   172.16.20.12   8443:31588/TCP      4m49s
kube-system   service/internal-pushprox-server            ClusterIP      10.96.232.144   <none>         8444/TCP            4m49s
kube-system   service/kube-apiserver                      LoadBalancer   10.96.232.180   172.16.20.10   443:30327/TCP       7m23s
kube-system   service/kube-dns                            ClusterIP      10.96.232.10    <none>         53/UDP,53/TCP       8m6s
kube-system   service/kube-state-metrics                  ClusterIP      10.96.232.71    <none>         9443/TCP            4m49s
kube-system   service/metrics-server                      ClusterIP      10.96.232.19    <none>         443/TCP             4m32s
kube-system   service/onprem-user-cluster-controller      ClusterIP      10.96.232.142   <none>         9090/TCP,443/TCP    3m41s
kube-system   service/seesaw-for-gke-admin-274b6vh8s2-1   ClusterIP      None            <none>         20257/TCP           8m
kube-system   service/stackdriver-operator                ClusterIP      10.96.232.107   <none>         9090/TCP            5m18s
kube-system   service/stackdriver-prometheus-k8s          ClusterIP      None            <none>         9090/TCP            5m2s
kube-system   service/vsphere-controller-manager          ClusterIP      10.96.232.28    <none>         9090/TCP            8m6s
kube-system   service/vsphere-metrics-exporter            ClusterIP      10.96.232.70    <none>         9090/TCP            4m47s

NAMESPACE     NAME                                       DESIRED   CURRENT   READY   UP-TO-DATE   AVAILABLE   NODE SELECTOR                                            AGE
kube-system   daemonset.apps/calico-node                 3         3         3       3            3           kubernetes.io/os=linux                                   8m5s
kube-system   daemonset.apps/kube-master-metrics-proxy   1         1         1       1            1           node-role.kubernetes.io/master=                          4m49s
kube-system   daemonset.apps/kube-proxy                  3         3         3       3            3           <none>                                                   8m1s
kube-system   daemonset.apps/node-exporter               2         2         2       2            2           kubernetes.io/os=linux                                   4m49s
kube-system   daemonset.apps/node-exporter-master        1         1         1       1            1           kubernetes.io/os=linux,node-role.kubernetes.io/master=   4m49s
kube-system   daemonset.apps/stackdriver-log-forwarder   3         3         3       3            3           kubernetes.io/os=linux                                   5m2s

NAMESPACE     NAME                                                       READY   UP-TO-DATE   AVAILABLE   AGE
kube-system   deployment.apps/calico-typha                               1/1     1            1           8m5s
kube-system   deployment.apps/citadel                                    1/1     1            1           4m49s
kube-system   deployment.apps/cluster-health-controller                  1/1     1            1           4m47s
kube-system   deployment.apps/clusterapi-controllers                     1/1     1            1           8m6s
kube-system   deployment.apps/gke-master-etcd-maintenance                1/1     1            1           5m18s
kube-system   deployment.apps/kube-dns                                   2/2     2            2           8m6s
kube-system   deployment.apps/kube-state-metrics                         1/1     1            1           4m49s
kube-system   deployment.apps/load-balancer-seesaw                       1/1     1            1           8m
kube-system   deployment.apps/metrics-server                             1/1     1            1           4m32s
kube-system   deployment.apps/metrics-server-operator                    1/1     1            1           4m56s
kube-system   deployment.apps/monitoring-operator                        1/1     1            1           5m5s
kube-system   deployment.apps/onprem-user-cluster-controller             1/1     1            1           3m41s
kube-system   deployment.apps/pushprox-server                            1/1     1            1           4m49s
kube-system   deployment.apps/stackdriver-metadata-agent-cluster-level   1/1     1            1           5m2s
kube-system   deployment.apps/stackdriver-operator                       1/1     1            1           5m18s
kube-system   deployment.apps/vsphere-metrics-exporter                   1/1     1            1           4m46s

NAMESPACE     NAME                                                                  DESIRED   CURRENT   READY   AGE
kube-system   replicaset.apps/calico-typha-78fd7798bb                               1         1         1       8m5s
kube-system   replicaset.apps/citadel-66dd66895b                                    1         1         1       4m49s
kube-system   replicaset.apps/cluster-health-controller-79548b44b                   1         1         1       4m47s
kube-system   replicaset.apps/clusterapi-controllers-5cd6c9bb47                     1         1         1       8m6s
kube-system   replicaset.apps/gke-master-etcd-maintenance-7f4fff496b                1         1         1       5m18s
kube-system   replicaset.apps/kube-dns-5bdb9f84d                                    2         2         2       8m6s
kube-system   replicaset.apps/kube-state-metrics-669d478d6b                         0         0         0       4m49s
kube-system   replicaset.apps/kube-state-metrics-69857cd5f6                         1         1         1       3m28s
kube-system   replicaset.apps/load-balancer-seesaw-56c46ccf85                       1         1         1       8m
kube-system   replicaset.apps/metrics-server-5f57b546db                             1         1         1       4m24s
kube-system   replicaset.apps/metrics-server-986848cd6                              0         0         0       4m32s
kube-system   replicaset.apps/metrics-server-operator-67d5c77897                    1         1         1       4m56s
kube-system   replicaset.apps/monitoring-operator-59d8d5f49c                        1         1         1       5m5s
kube-system   replicaset.apps/onprem-user-cluster-controller-784bbf9bff             1         1         1       3m41s
kube-system   replicaset.apps/pushprox-server-6f55784c5f                            1         1         1       4m42s
kube-system   replicaset.apps/pushprox-server-6f6b97b74c                            0         0         0       4m49s
kube-system   replicaset.apps/stackdriver-metadata-agent-cluster-level-7d59864ffb   1         1         1       5m2s
kube-system   replicaset.apps/stackdriver-operator-669b47ccfb                       1         1         1       5m18s
kube-system   replicaset.apps/vsphere-metrics-exporter-647db699f7                   1         1         1       4m46s

NAMESPACE     NAME                                          READY   AGE
kube-system   statefulset.apps/stackdriver-prometheus-k8s   1/1     5m2s
```

## CRDs
```
ubuntu@gke-admin-ws-210517-022057:~$ kubectl get crds --kubeconfig kubeconfig
NAME                                                         CREATED AT
applications.app.k8s.io                                      2021-05-18T04:43:30Z
bgpconfigurations.crd.projectcalico.org                      2021-05-18T04:40:43Z
bgppeers.crd.projectcalico.org                               2021-05-18T04:40:43Z
blockaffinities.crd.projectcalico.org                        2021-05-18T04:40:47Z
bundlebuilders.bundle.gke.io                                 2021-05-18T04:40:20Z
bundles.bundle.gke.io                                        2021-05-18T04:40:20Z
clusterbundles.bundle.gke.io                                 2021-05-18T04:40:20Z
clusterinformations.crd.projectcalico.org                    2021-05-18T04:40:44Z
clusters.cluster.k8s.io                                      2021-05-18T04:40:41Z
componentbuilders.bundle.gke.io                              2021-05-18T04:40:20Z
componentlists.bundle.gke.io                                 2021-05-18T04:40:20Z
components.bundle.gke.io                                     2021-05-18T04:40:20Z
componentsets.bundle.gke.io                                  2021-05-18T04:40:20Z
felixconfigurations.crd.projectcalico.org                    2021-05-18T04:40:43Z
gkeonprembundles.bundle.gke.io                               2021-05-18T04:40:20Z
globalnetworkpolicies.crd.projectcalico.org                  2021-05-18T04:40:45Z
globalnetworksets.crd.projectcalico.org                      2021-05-18T04:40:45Z
hostendpoints.crd.projectcalico.org                          2021-05-18T04:40:44Z
ipamblocks.crd.projectcalico.org                             2021-05-18T04:40:46Z
ipamconfigs.crd.projectcalico.org                            2021-05-18T04:40:47Z
ipamhandles.crd.projectcalico.org                            2021-05-18T04:40:47Z
ippools.crd.projectcalico.org                                2021-05-18T04:40:43Z
machineclasses.cluster.k8s.io                                2021-05-18T04:40:42Z
machinedeployments.cluster.k8s.io                            2021-05-18T04:40:41Z
machines.cluster.k8s.io                                      2021-05-18T04:40:41Z
machinesets.cluster.k8s.io                                   2021-05-18T04:40:41Z
metricsserver.addons.k8s.io                                  2021-05-18T04:43:52Z
monitoring.addons.k8s.io                                     2021-05-18T04:43:43Z
networkpolicies.crd.projectcalico.org                        2021-05-18T04:40:46Z
networksets.crd.projectcalico.org                            2021-05-18T04:40:45Z
nodeconfigs.bundleext.gke.io                                 2021-05-18T04:40:20Z
onpremnodepools.onprem.cluster.gke.io                        2021-05-18T04:45:07Z
onpremuserclusters.onprem.cluster.gke.io                     2021-05-18T04:45:07Z
packagedeploymentclasses.bundle.gke.io                       2021-05-18T04:40:20Z
packagedeployments.bundle.gke.io                             2021-05-18T04:40:20Z
patchtemplatebuilders.bundle.gke.io                          2021-05-18T04:40:20Z
patchtemplates.bundle.gke.io                                 2021-05-18T04:40:20Z
requirements.bundle.gke.io                                   2021-05-18T04:40:20Z
seesawgroups.seesaw.gke.io                                   2021-05-18T04:40:48Z
stackdrivers.addons.sigs.k8s.io                              2021-05-18T04:43:30Z
vsphereclusterproviderconfigs.vsphereproviderconfig.k8s.io   2021-05-18T04:40:41Z
vspheremachineproviderconfigs.vsphereproviderconfig.k8s.io   2021-05-18T04:40:41Z
```