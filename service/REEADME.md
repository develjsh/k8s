# service
Service는 Pod의 논리적 집합이며, 어떻게 접근할지에 대한 정책을 정의 해놓은 것을 말합니다.  
Label Selector를 통해 어떤 Pod를 포함할지 정의가 가능합니다.  
또한 Pod들을 통해 실행되고 있는 애플리케이션을 네트워크에 노출시키는 가상의 컴포넌트입니다.  
Kubenetes 내부의 다양한 객체들이 애플리케이션과 연결할 때, 애플리케이션이 다른 외부의 애플리케이션 연결할 때, 다른 외부의 애플리케이션이나 사용자와 연결될 수 있도록 도와주는 역활을 합니다.  

## Service 유형
Service 유형은 크게 4 가지로 분류됩니다.  
1. ClusterIP(기본 형태)  
    클러스터 내부에서만 접근 가능한 IP 입니다.  
2. NodePort  
    Port 번호를 통해 외부에서 접근 가능합니다.(NAT 컨셉)  
3. LoadBalancer  
    외부의 Load Balancer를 사용하는 방법입니다.     
4. ExternalName  
    kube-dns 컴포넌트로 DNS를 이용하는 방법입니다.  