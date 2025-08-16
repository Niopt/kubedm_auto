**Niopt Kubernetes Cluster Automation**

Описание:
- Эта коллекция Ansible предназначена для автоматизации развертывания кластера Kubernetes с помощью kubeadm. Она обеспечивает установку мастер-ноды и присоединение рабочих нод к кластеру.

**Состав коллекции**

Коллекция состоит из двух ролей:

1) master_node – Устанавливает мастер-ноду Kubernetes.

- Инициализирует кластер с помощью kubeadm init.

- Настраивает необходимые компоненты и сеть кластера.

- Генерирует команду kubeadm join для присоединения рабочих нод.

2) work_node – Устанавливает рабочую ноду и присоединяет её к существующему кластеру.

- Устанавливает Kubernetes на рабочей ноде.

- Выполняет присоединение к кластеру с использованием kubeadm join, предоставленного мастер-нодой.


**Niopt Kubernetes Cluster Automation**

Description:
- This Ansible collection is designed to automate the deployment of a Kubernetes cluster using kubeadm. It installs a master node and joins worker nodes to the cluster.

**Collection Contents**

The collection consists of two roles:

1) master_node – Installs a Kubernetes master node.

- Initializes the cluster using kubeadm init.

- Configures the required components and cluster network.

- Generates the kubeadm join command to join worker nodes.

2) work_node – Installs a worker node and joins it to an existing cluster.

- Installs Kubernetes on the worker node.

- Joins the cluster using kubeadm join provided by the master node.
