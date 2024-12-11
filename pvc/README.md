# pvc

## 궁금한 것들
- pvc는 namespace 설정이 가능한가?  
가능합니다.  

- spec.accessModes 종류는? 
ReadWriteOnce: 한 노드에서 읽기/쓰기 가능.  
ReadOnlyMany: 여러 노드에서 읽기만 가능.  
ReadWriteMany: 여러 노드에서 읽기/쓰기 가능.  