
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:aecf593217b6ba39bf6e9f99adccb50a130ce2debbdd2e90cf82afc35eb08ef3 |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:ca90553412d96a2a6c3ceb4161a5c29facb3bb5d61ad96519ce6ad9e37627ed6 |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:05948ccd999cfa4646cb022e2da0185dd0c46f1d1945ceab569857e213cb256f |

## IBM Storage Scale images acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:e7366f5fa4ca7dbcd71b2e8966a4e795d78c0c9c2167b33088b5565f29ab591d |
| workerX/masterX* | config | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:e7366f5fa4ca7dbcd71b2e8966a4e795d78c0c9c2167b33088b5565f29ab591d |
| workerX/masterX* | gpfs (Data Access Edition) | cp.icr.io/cp/spectrum/scale/data-access | ibm-spectrum-scale-daemon@sha256:4fc35e16ca8d8fa39f68e139f550679fddee37636c0fb3900b7b4f2bac723337 |
| workerX/masterX* | gpfs (Data Management Edition) | cp.icr.io/cp/spectrum/scale/data-management | ibm-spectrum-scale-daemon@sha256:aea1cac9a5c5b66ef17e31f469a1eceb12b456e647d172c9583d0c1e1d63ef69 |
| workerX/masterX* | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:582e18f13291d7c686ec4e6e92d20b24c62ae0fc72767c46f30a69b1a6198055  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-gui@sha256:31c2aebcd5f95c99ae3c03b41af17dc4e6523caca12635cc5f161d51dba107a6 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:a5996e1d0eb2bcdac2009c696c4f9f23e9e40273fc305562ec077463ecd18a99 |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/spectrum/scale | postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:582e18f13291d7c686ec4e6e92d20b24c62ae0fc72767c46f30a69b1a6198055 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-pmcollector@sha256:79237b6ad3076722520e7743841e87148de241e32a0bc7e7cc2bc5b6a4e52fff |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:a5996e1d0eb2bcdac2009c696c4f9f23e9e40273fc305562ec077463ecd18a99 |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-grafana-bridge@sha256:fca0c3bdfb2e3161b134548e9daa66df71289ab048ce52328fbfa50b3c8ed56e |
| coredns-XXXXX | coredns | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-coredns@sha256:1ba4d51e896607c6f968f8df8e04ccfe7a71babd778838c9de040beda6bf1ff7 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/spectrum/scale/csi | csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/spectrum/scale/csi | csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/spectrum/scale/csi | csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/spectrum/scale/csi | livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/spectrum/scale/csi | csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/spectrum/scale/csi | csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/spectrum/scale/csi | ibm-spectrum-scale-csi-driver@sha256:34925dffe24be39e19fda24339bed15c7e9e10110285b11aab304df6bf40a0ec |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:aecf593217b6ba39bf6e9f99adccb50a130ce2debbdd2e90cf82afc35eb08ef3
cp.icr.io/cp/spectrum/scale/data-access/ibm-spectrum-scale-daemon@sha256:4fc35e16ca8d8fa39f68e139f550679fddee37636c0fb3900b7b4f2bac723337
cp.icr.io/cp/spectrum/scale/data-management/ibm-spectrum-scale-daemon@sha256:aea1cac9a5c5b66ef17e31f469a1eceb12b456e647d172c9583d0c1e1d63ef69
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-core-init@sha256:e7366f5fa4ca7dbcd71b2e8966a4e795d78c0c9c2167b33088b5565f29ab591d
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmcollector@sha256:79237b6ad3076722520e7743841e87148de241e32a0bc7e7cc2bc5b6a4e52fff
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-monitor@sha256:a5996e1d0eb2bcdac2009c696c4f9f23e9e40273fc305562ec077463ecd18a99
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-gui@sha256:31c2aebcd5f95c99ae3c03b41af17dc4e6523caca12635cc5f161d51dba107a6
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-grafana-bridge@sha256:fca0c3bdfb2e3161b134548e9daa66df71289ab048ce52328fbfa50b3c8ed56e
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:05948ccd999cfa4646cb022e2da0185dd0c46f1d1945ceab569857e213cb256f
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-coredns@sha256:1ba4d51e896607c6f968f8df8e04ccfe7a71babd778838c9de040beda6bf1ff7
cp.icr.io/cp/spectrum/scale/ubi-minimal@sha256:582e18f13291d7c686ec4e6e92d20b24c62ae0fc72767c46f30a69b1a6198055
cp.icr.io/cp/spectrum/scale/postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:ca90553412d96a2a6c3ceb4161a5c29facb3bb5d61ad96519ce6ad9e37627ed6
cp.icr.io/cp/spectrum/scale/csi/ibm-spectrum-scale-csi-driver@sha256:34925dffe24be39e19fda24339bed15c7e9e10110285b11aab304df6bf40a0ec
cp.icr.io/cp/spectrum/scale/csi/csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2
cp.icr.io/cp/spectrum/scale/csi/csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f
cp.icr.io/cp/spectrum/scale/csi/csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1
cp.icr.io/cp/spectrum/scale/csi/csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af
cp.icr.io/cp/spectrum/scale/csi/livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce
cp.icr.io/cp/spectrum/scale/csi/csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0
```
