# pv


## 궁금한 것들
- pv는 namespace 설정이 가능한가?
PersistentVolume(PV) 리소스는 클러스터 범위의 리소스로, 네임스페이스와 관계없이 사용할 수 있도록 설계되었습니다. 따라서 PersistentVolume에는 네임스페이스를 설정할 수 없고, metadata.namespace 필드도 지원되지 않습니다.