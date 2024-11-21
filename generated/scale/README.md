
# Container image list for IBM Storage Scale container native

## IBM Storage Scale images acquired from nonentitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through the IBM Container Repository that do not require entitlement. These images can be anonymously pulled.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| ibm-spectrum-scale-controller-manager-XXXXXXXXX-XXXXX | manager | icr.io/cpopen | ibm-spectrum-scale-operator@sha256:dd543baefcb9ec4db696b63c3a1c2b318146f9837c8cf4f4ccabaee7b95a10ec |
| ibm-spectrum-scale-csi-operator | operator | icr.io/cpopen  | ibm-spectrum-scale-csi-operator@sha256:f40465313a11a0567d7f708d8b0430c89d163bf334bddbf3012fe47c129b7dcc |
| must-gather-XXXXX | must-gather | icr.io/cpopen | ibm-spectrum-scale-must-gather@sha256:b4c78d4b3e4d725af5e4b7c59ffeb7988dfda940e03a0f0d0fcd752c2523a9ad |

## IBM Storage Scale images acquired from entitled IBM Container Repository

The images that are listed in the following table are the container images that are obtained through entitlement to the IBM Container Repository.

| Pod | Container | Repository | Image |
|-----|-----------|------------|---------------------|
| workerX/masterX* | mmbuildgpl | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:9246869945e9f7e023b49cc2380b372bc826318349474befdbdbd4efce25ca4e |
| workerX/masterX* | config | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-core-init@sha256:9246869945e9f7e023b49cc2380b372bc826318349474befdbdbd4efce25ca4e |
| workerX/masterX* | gpfs (Data Access Edition) | cp.icr.io/cp/spectrum/scale/data-access | ibm-spectrum-scale-daemon@sha256:40b1e7287f8d32e8757857cc6d031f0c28c90cf8e43e821aa6a122b9934b5f38 |
| workerX/masterX* | gpfs (Data Management Edition) | cp.icr.io/cp/spectrum/scale/data-management | ibm-spectrum-scale-daemon@sha256:e68c28ecfe1537131a2acb688dbb96e58bfa49025c5d033b1c97078291966d75 |
| workerX/masterX* | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:c0e70387664f30cd9cf2795b547e4a9a51002c44a4a86aa9335ab030134bf392  |
| ibm-spectrum-scale-gui-X | liberty | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-gui@sha256:9de0a7674cc1a99e6275c00e0e90106a1035d4c18a008ceda72595e5d7058541 |
| ibm-spectrum-scale-gui-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:1d6f783d24ad5169bd0496b52521af09a98b9dc0994e9f56bffbbd2520c879fe |
| ibm-spectrum-scale-gui-X | postgres | cp.icr.io/cp/spectrum/scale | postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670 |
| ibm-spectrum-scale-gui-X | logs | cp.icr.io/cp/spectrum/scale | ubi-minimal@sha256:c0e70387664f30cd9cf2795b547e4a9a51002c44a4a86aa9335ab030134bf392 |
| ibm-spectrum-scale-pmcollector-X | pmcollector | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-pmcollector@sha256:41a0834dc6bae6673421e3099791bb2e78dc3fd427d8243b4047f5a1e358df59 |
| ibm-spectrum-scale-pmcollector-X | sysmon | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-monitor@sha256:1d6f783d24ad5169bd0496b52521af09a98b9dc0994e9f56bffbbd2520c879fe |
| ibm-spectrum-scale-grafana-bridge-X | grafanabridge | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-grafana-bridge@sha256:05b8e9c8422e8a04e742d23cce86e2179db5253625a73445852a21663432f8b5 |
| coredns-XXXXX | coredns | cp.icr.io/cp/spectrum/scale | ibm-spectrum-scale-coredns@sha256:1ba4d51e896607c6f968f8df8e04ccfe7a71babd778838c9de040beda6bf1ff7 |
| ibm-spectrum-scale-csi-snapshotter | csi-snapshotter | cp.icr.io/cp/spectrum/scale/csi | csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2  |
| ibm-spectrum-scale-csi-attacher | ibm-spectrum-scale-csi-attacher | cp.icr.io/cp/spectrum/scale/csi | csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af |
| ibm-spectrum-scale-csi-provisioner | csi-provisioner | cp.icr.io/cp/spectrum/scale/csi | csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f |
| ibm-spectrum-scale-csi-driver-XXXXX | liveness-probe | cp.icr.io/cp/spectrum/scale/csi | livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce |
| ibm-spectrum-scale-csi-driver-XXXXX | driver-registrar | cp.icr.io/cp/spectrum/scale/csi | csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1 |
| ibm-spectrum-scale-csi-resizer-X | ibm-spectrum-scale-csi-resizer | cp.icr.io/cp/spectrum/scale/csi | csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0 |
| ibm-spectrum-scale-csi-driver-XXXXX | ibm-spectrum-scale-csi | cp.icr.io/cp/spectrum/scale/csi | ibm-spectrum-scale-csi-driver@sha256:8443cb08d51803a741d3db1ecbbc5e56741bb2e34bb35d63eff0832fdc48e6ca |

*Pod names that contain the mmbuildgpl, config, and gpfs containers may vary. The pod name is based on the shortname of the node that it was scheduled to.

>**NOTE:** This list is for information only.

## Air gapped

When setting up your environment to be air-gapped, use `skopeo` to copy the following images from the IBM Entitled Container Registry to your internal production-grade image registry. For more information, see [Skopeo Copy to the Rescue](https://www.redhat.com/en/blog/skopeo-copy-rescue).

```bash
# IBM Storage Scale container native images
icr.io/cpopen/ibm-spectrum-scale-operator@sha256:dd543baefcb9ec4db696b63c3a1c2b318146f9837c8cf4f4ccabaee7b95a10ec
cp.icr.io/cp/spectrum/scale/data-access/ibm-spectrum-scale-daemon@sha256:40b1e7287f8d32e8757857cc6d031f0c28c90cf8e43e821aa6a122b9934b5f38
cp.icr.io/cp/spectrum/scale/data-management/ibm-spectrum-scale-daemon@sha256:e68c28ecfe1537131a2acb688dbb96e58bfa49025c5d033b1c97078291966d75
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-core-init@sha256:9246869945e9f7e023b49cc2380b372bc826318349474befdbdbd4efce25ca4e
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-coredns@sha256:1ba4d51e896607c6f968f8df8e04ccfe7a71babd778838c9de040beda6bf1ff7
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-grafana-bridge@sha256:05b8e9c8422e8a04e742d23cce86e2179db5253625a73445852a21663432f8b5
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-gui@sha256:9de0a7674cc1a99e6275c00e0e90106a1035d4c18a008ceda72595e5d7058541
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-monitor@sha256:1d6f783d24ad5169bd0496b52521af09a98b9dc0994e9f56bffbbd2520c879fe
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmcollector@sha256:41a0834dc6bae6673421e3099791bb2e78dc3fd427d8243b4047f5a1e358df59
cp.icr.io/cp/spectrum/scale/ibm-spectrum-scale-pmsensors@sha256:93b63e92eed5b69dfd7b6306635b618c868073b8cc8cdf3767404810fc250c90
cp.icr.io/cp/spectrum/scale/postgres@sha256:b2f06ce12103bedbc0a49ae4ffff062d90824e0f45462de712f66952679f7670
cp.icr.io/cp/spectrum/scale/ubi-minimal@sha256:c0e70387664f30cd9cf2795b547e4a9a51002c44a4a86aa9335ab030134bf392
icr.io/cpopen/ibm-spectrum-scale-must-gather@sha256:b4c78d4b3e4d725af5e4b7c59ffeb7988dfda940e03a0f0d0fcd752c2523a9ad
# IBM Container Storage Interface (CSI) images
icr.io/cpopen/ibm-spectrum-scale-csi-operator@sha256:f40465313a11a0567d7f708d8b0430c89d163bf334bddbf3012fe47c129b7dcc
cp.icr.io/cp/spectrum/scale/csi/csi-attacher@sha256:4eb73137b66381b7b5dfd4d21d460f4b4095347ab6ed4626e0199c29d8d021af
cp.icr.io/cp/spectrum/scale/csi/csi-node-driver-registrar@sha256:f6717ce72a2615c7fbc746b4068f788e78579c54c43b8716e5ce650d97af2df1
cp.icr.io/cp/spectrum/scale/csi/csi-provisioner@sha256:d078dc174323407e8cc6f0f9abd4efaac5db27838f1564d0253d5e3233e3f17f
cp.icr.io/cp/spectrum/scale/csi/csi-resizer@sha256:2e2b44393539d744a55b9370b346e8ebd95a77573064f3f9a8caf18c22f4d0d0
cp.icr.io/cp/spectrum/scale/csi/csi-snapshotter@sha256:becc53e25b96573f61f7469923a92fb3e9d3a3781732159954ce0d9da07233a2
cp.icr.io/cp/spectrum/scale/csi/ibm-spectrum-scale-csi-driver@sha256:8443cb08d51803a741d3db1ecbbc5e56741bb2e34bb35d63eff0832fdc48e6ca
cp.icr.io/cp/spectrum/scale/csi/livenessprobe@sha256:4dc0b87ccd69f9865b89234d8555d3a614ab0a16ed94a3016ffd27f8106132ce
```
