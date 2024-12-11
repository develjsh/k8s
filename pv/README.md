# pv

## 궁금한 것들
- pv는 namespace 설정이 가능한가?  
PersistentVolume(PV) 리소스는 클러스터 범위의 리소스로, 네임스페이스와 관계없이 사용할 수 있도록 설계되었습니다. 따라서 PersistentVolume에는 네임스페이스를 설정할 수 없고, metadata.namespace 필드도 지원되지 않습니다.

- storageClassName?  
storageClassName은 Kubernetes에서 스토리지를 동적으로 관리하고 프로비저닝하는 방법을 정의하는 StorageClass 리소스의 이름입니다. PersistentVolume(PV)와 PersistentVolumeClaim(PVC)에서 이 필드를 사용하여 특정 스토리지 클래스를 지정할 수 있습니다.  
PVC가 요청하는 storageClassName과 일치하는 StorageClass의 설정에 따라 PV가 동적으로 생성되거나 PVC가 적합한 PV에 바인딩됩니다.  
