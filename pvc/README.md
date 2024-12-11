# pvc

## 중요한 것
- pv와 accessMode가 같아야 합니다.  

## 궁금한 것들
- pvc는 namespace 설정이 가능한가?  
가능합니다.  

- spec.accessModes 종류는?  
ReadWriteOnce: 한 노드에서 읽기/쓰기 가능.  
ReadOnlyMany: 여러 노드에서 읽기만 가능.  
ReadWriteMany: 여러 노드에서 읽기/쓰기 가능.  

- pod에 연결할려면?  
pod 정의 YAML에서 volumes와 volumeMounts를 설정해줘야 합니다.  
설정 방법은 simple-pod에 작업했습니다.  
*pvc namespace는 pod의 namespace와 동일해야 합니다.  

