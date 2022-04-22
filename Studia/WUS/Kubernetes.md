## Kubernetes

![ilustracja](https://upload.wikimedia.org/wikipedia/commons/b/be/Kubernetes.png)

**Node** - wirtualna maszyna (serwer dla node'ów)
**Pod** - najmniejsza jednostka wykonawcza w K8s jeden lub kilka kontenerów (zazwyczaj jeden kontener xd)
**Service** - abstrakcyjny obiekt, który definiuje logiczny zbiór podów i polityke dostępów do nich (to definiujemy w yamlu)
**Deployment** - definicja porządanego stanu Podów (definiuje service)
**NameSpace** - przestrzeń nazw obiektów


### Kubernetes master node (Control plane)
Jego zadaniem jest zarządzanie danym clustrem

- **kube-scheduler** - przyporzadkowuje Pod do danego Node
- **etcd** - baza danych klucz-wartosc
- **kube-controller-manager** - kilka kontrolerów, do każdego z pojęć (node, api). Sprawdza on stany wszystkich obiektów i reaguje jeżeli jest za mało nodów itp
- **cloud-controller-manager** (nie mylic z kube-controller-managerem) - interfejs do chmury  

<br>

### Cykl życia Poda - fazy
![[Cykla zycia poda.png]]


**ConfigMap** - hashmapa configów 

### Rodzaje komunikacja

