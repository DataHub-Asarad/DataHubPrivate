<a href="https://ssenerg.com">
    <div style="margin-bottom:1em;"> 
        <img style="margin-right:-.2em;" align="left" src="https://i.postimg.cc/3wwHhJvM/logo-dh.png" title="SSENERG" width="100" height="100"/>
    </div>
    <div style="margin-bottom:-1.5em;">
        <h1 display="display:inline;">
            <font size="+4">DataHub</font>
        </h1>
    </div>
</a>

<div style="margin-left:5em;">
    <span style="vertical-align: middle;"><font size="+2">Horizontaly scaled and modular product for fetching and providing live and historical data from any Exchange containing many additional services with completely automated deployment</font></span>
</div>

---

# Product Structure
#### DataHub directory
```
  │
  ├── Manager
  │   ├── ci-cd.sh
  │   ├── manual.sh
  |   └── ...
  │
  ├── Initial 
  │   └── DynamicProvisioning
  │       ├── Ceph
  │       └── StorageClass
  │
  ├── Resources
  |   ├── Routing
  |   ├── CertManager
  |   ├── MetalLb
  |   ├── ExternalDNS
  |   ├── IngressNginx
  |   ├── MariaGalera
  |   ├── Quest
  |   ├── NatsJetstream
  |   ├── LDAP
  |   ├── Kerberos
  |   ├── Prometheus
  |   └── ELK
  │
  ├── DjangoPrivate
  │   ├── Updater
  │   ├── Producer 
  │   ├── Consumer 
  │   ├── CoreFeaturesLab 
  │   ├── CoreEngine
  |   └── PlayGround
  │
  └── DjangoPublic
      ├── MyPanel 
      ├── Provider 
      ├── BackTester 
      ├── FeaturesLab 
      ├── Executer 
      └── AI 
```

---

# Requirements
- **Kubernetes Cluster** v1.28.2
- **Initial Configs**
    - Deploy manually Initial Repository
- **Helm** v3.10.1
- **Python** v3.10.12
- **virtualenv** v20.24.7
- **BWS CLI** v0.3.1

--- 

# Clone

```bash
# ------- DataHub - Private
git clone git@github.com:DataHub-Asarad/.github-private.git DataHub && cd DataHub

# ------- DataHub - Public
git clone git@github.com:DataHub-Asarad/.github.git DataHubPublic

# ------- Manager
git clone git@github.com:DataHub-Asarad/Manager.git

# ------- Initial
git clone git@github.com:DataHub-Asarad/Initial.git

# ------- Resources
git clone git@github.com:DataHub-Asarad/Resources.git && cd Resources
git clone git@github.com:DataHub-Asarad/Routing.git
git clone git@github.com:DataHub-Asarad/CertManager.git
git clone git@github.com:DataHub-Asarad/MetalLb.git
git clone git@github.com:DataHub-Asarad/ExternalDNS.git
git clone git@github.com:DataHub-Asarad/IngressNginx.git
git clone git@github.com:DataHub-Asarad/MariaGalera.git
git clone git@github.com:DataHub-Asarad/Quest.git
git clone git@github.com:DataHub-Asarad/NatsJetstream.git
git clone git@github.com:DataHub-Asarad/LDAP.git
git clone git@github.com:DataHub-Asarad/Kerberos.git
git clone git@github.com:DataHub-Asarad/Prometheus.git
git clone git@github.com:DataHub-Asarad/ELK.git

# ------- Django - Private
git clone git@github.com:DataHub-Asarad/DjangoPrivate.git && cd ../DjangoPrivate
git clone git@github.com:DataHub-Asarad/Updater.git
git clone git@github.com:DataHub-Asarad/Producer.git
git clone git@github.com:DataHub-Asarad/Consumer.git
git clone git@github.com:DataHub-Asarad/CoreFeaturesLab.git
git clone git@github.com:DataHub-Asarad/CoreEngine.git
git clone git@github.com:DataHub-Asarad/PlayGround.git

# ------- Django - Public
git clone git@github.com:DataHub-Asarad/DjangoPublic.git && cd ../DjangoPublic
git clone git@github.com:DataHub-Asarad/MyPanel.git
git clone git@github.com:DataHub-Asarad/Provider.git
git clone git@github.com:DataHub-Asarad/BackTester.git
git clone git@github.com:DataHub-Asarad/FeaturesLab.git
git clone git@github.com:DataHub-Asarad/Executer.git
git clone git@github.com:DataHub-Asarad/AI.git
```

---

# Installation
After Clonnig all the repositories, you should install the product by Manager pipeline:
```bash
echo "alis cicd='source ~/DataHub/Manager/ci-cd.sh'" >> ~/.bashrc
echo "alis manual='source ~/DataHub/Manager/manual.sh'" >> ~/.bashrc
```
and then install Initial repository manually:
```bash
TODO
```

---

# How to Deploy? **:)**
```bash
# CI/CD  Deployment
cicd   
# Manual Deployment
manual
```
