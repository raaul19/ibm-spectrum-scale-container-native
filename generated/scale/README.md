
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:9a87ce8dda3d461eb48fc47f6b7c7e43e31f64918acd68cc5c89818e8a1fe309 |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:b93ac6b84a5d538fce576c8182f63c7f5d377df3a05c71b8ec64ed664ad30a25 |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:655296105968d876901bdc9db735aa52d417dfeeb737fd03e79a27260962b163 |
{: caption="Images (non-entitled)" caption-side="bottom"}

## IBM Storage Scale images that are acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:1e1f7c53efed9b50833570ca6b29c03305b02b3ceeb391848bad29c75e36ddf7 |
| workerX/masterX* | config | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:1e1f7c53efed9b50833570ca6b29c03305b02b3ceeb391848bad29c75e36ddf7 |
| workerX/masterX* | gpfs (if using Data Access Edition) | cp.icr.io/cp/spectrum/scale/data-access | ibm-spectrum-scale-daemon@sha256:0ee38f491170ca6528644331dc6f1b6aedff1abd8a1ae0796fe48bf8a6fb011c |
| workerX/masterX* | gpfs (if using Data Management Edition) | cp.icr.io/cp/spectrum/scale/data-management | ibm-spectrum-scale-daemon@sha256:02cfe2e798dc0092930723eb36d894a84d42905946f755d2abb000b9ce513f3f |
| workerX/masterX* | logs | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-logs@sha256:5dd3ef4f95dfa19c3a72103e90732266e95114ea1e65762ff844c96adadee329  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-gui@sha256:44c2e3bb807b9a8724301f0bbe9014b0c53d4a8efa161554efb6a7ec8e85131e |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:27cdeaa43caceafc60cd5cf6f373d1f0a6661e852896094fdc9c0daf005691f3 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/spectrum/scale | postgres@sha256:bbd7346fab25b7e0b25f214829d6ebfb78ef0465059492e46dee740ce8fcd844 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-logs@sha256:5dd3ef4f95dfa19c3a72103e90732266e95114ea1e65762ff844c96adadee329 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-pmcollector@sha256:f7a284866a968c7ad20e752d76610491e08348647a3ee249057dadd4e105d57e |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:27cdeaa43caceafc60cd5cf6f373d1f0a6661e852896094fdc9c0daf005691f3 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/spectrum/scale/csi | csi-snapshotter@sha256:2e04046334baf9be425bb0fa1d04c2d1720d770825eedbdbcdb10d430da4ad8c  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/spectrum/scale/csi | csi-attacher@sha256:b4d611100ece2f9bc980d1cb19c2285b8868da261e3b1ee8f45448ab5512ab94 |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/spectrum/scale/csi | csi-provisioner@sha256:bf5a235b67d8aea00f5b8ec24d384a2480e1017d5458d8a63b361e9eeb1608a9 |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/spectrum/scale/csi | livenessprobe@sha256:5baeb4a6d7d517434292758928bb33efc6397368cbb48c8a4cf29496abf4e987 |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/spectrum/scale/csi | csi-node-driver-registrar@sha256:f25af73ee708ff9c82595ae99493cdef9295bd96953366cddf36305f82555dac |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/spectrum/scale/csi | csi-resizer@sha256:a541e6cc2d8b011bb21b1d4ffec6b090e85270cce6276ee302d86153eec0af43 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/spectrum/scale/csi | ibm-spectrum-scale-csi-driver@sha256:96e3264bc922826d6f3e8e3d3be4d010c67f65cf5b16e2acadd5ae75258e3ef3 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-grafana-bridge@sha256:603f3a47d31f7f33671b013efc5c5f82f1208350415e1850877115c9bd04d557 |
| coredns-XXXXX | coredns | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-coredns@sha256:88cbfe40fd302a6467cb7e852b298f6c8d8659782ab313706d491d3ddf172a6e |
{: caption="Images (entitled)" caption-side="bottom"}

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

For air-gapped support, a production-grade Docker V2 registry that is available and accessible from the Red Hat OpenShift Container Platform cluster nodes is required. This might be such registry as Quay Enterprise, JFrog Artifactory, or Docker Registry. The Red Hat OpenShift Internal Registry is not supported.

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:9a87ce8dda3d461eb48fc47f6b7c7e43e31f64918acd68cc5c89818e8a1fe309
cp.icr.io/cp/spectrum/scale/data-access/ibm-spectrum-scale-daemon@sha256:0ee38f491170ca6528644331dc6f1b6aedff1abd8a1ae0796fe48bf8a6fb011c
cp.icr.io/cp/spectrum/scale/data-management/ibm-spectrum-scale-daemon@sha256:02cfe2e798dc0092930723eb36d894a84d42905946f755d2abb000b9ce513f3f
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-core-init@sha256:1e1f7c53efed9b50833570ca6b29c03305b02b3ceeb391848bad29c75e36ddf7
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-coredns@sha256:88cbfe40fd302a6467cb7e852b298f6c8d8659782ab313706d491d3ddf172a6e
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-grafana-bridge@sha256:603f3a47d31f7f33671b013efc5c5f82f1208350415e1850877115c9bd04d557
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-gui@sha256:44c2e3bb807b9a8724301f0bbe9014b0c53d4a8efa161554efb6a7ec8e85131e
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-logs@sha256:5dd3ef4f95dfa19c3a72103e90732266e95114ea1e65762ff844c96adadee329
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-monitor@sha256:27cdeaa43caceafc60cd5cf6f373d1f0a6661e852896094fdc9c0daf005691f3
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmcollector@sha256:f7a284866a968c7ad20e752d76610491e08348647a3ee249057dadd4e105d57e
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmsensors@sha256:45be0a941bd66619e56c5880186f5e59a5d288c658e39f6b69aaf71441683285
cp.icr.io/cp/spectrum/scale/postgres@sha256:bbd7346fab25b7e0b25f214829d6ebfb78ef0465059492e46dee740ce8fcd844
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:655296105968d876901bdc9db735aa52d417dfeeb737fd03e79a27260962b163
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:b93ac6b84a5d538fce576c8182f63c7f5d377df3a05c71b8ec64ed664ad30a25
cp.icr.io/cp/spectrum/scale/csi/csi-attacher@sha256:b4d611100ece2f9bc980d1cb19c2285b8868da261e3b1ee8f45448ab5512ab94
cp.icr.io/cp/spectrum/scale/csi/csi-node-driver-registrar@sha256:f25af73ee708ff9c82595ae99493cdef9295bd96953366cddf36305f82555dac
cp.icr.io/cp/spectrum/scale/csi/csi-provisioner@sha256:bf5a235b67d8aea00f5b8ec24d384a2480e1017d5458d8a63b361e9eeb1608a9
cp.icr.io/cp/spectrum/scale/csi/csi-resizer@sha256:a541e6cc2d8b011bb21b1d4ffec6b090e85270cce6276ee302d86153eec0af43
cp.icr.io/cp/spectrum/scale/csi/csi-snapshotter@sha256:2e04046334baf9be425bb0fa1d04c2d1720d770825eedbdbcdb10d430da4ad8c
cp.icr.io/cp/spectrum/scale/csi/ibm-spectrum-scale-csi-driver@sha256:96e3264bc922826d6f3e8e3d3be4d010c67f65cf5b16e2acadd5ae75258e3ef3
cp.icr.io/cp/spectrum/scale/csi/livenessprobe@sha256:5baeb4a6d7d517434292758928bb33efc6397368cbb48c8a4cf29496abf4e987
```

