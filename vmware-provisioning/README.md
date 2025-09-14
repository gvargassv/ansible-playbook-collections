# VMware Provisioning with Ansible

Este repositorio contiene un playbook y un rol de Ansible para **provisionar máquinas virtuales en VMware vSphere** de forma automatizada.  
Está diseñado para ejecutarse en **Ansible Automation Platform (AAP)** o en **AWX**.

## 🚀 Funcionalidad
- Creación de VMs basadas en parámetros definidos por variables.
- Configuración flexible de CPU, RAM, disco y red.
- Compatible con `community.vmware`.

## 📂 Estructura
- `inventories/` → Inventario Ansible.
- `playbooks/` → Playbook principal.
- `roles/vmware_vm_provision/` → Rol con lógica para crear la VM.
- `collections/requirements.yml` → Dependencias de colección.

## ⚙️ Variables principales
Se pueden modificar en `roles/vmware_vm_provision/defaults/main.yml` o pasar por **extra_vars** en AAP:

```yaml
vcenter_hostname: "vcenter.lab.local"
vcenter_username: "administrator@vsphere.local"
vcenter_password: "password"
vcenter_datacenter: "Datacenter01"
vcenter_cluster: "Cluster01"
vcenter_datastore: "Datastore01"
vcenter_network: "VM Network"
vm_name: "ansible-vm"
vm_num_cpus: 2
vm_memory_mb: 2048
vm_disk_gb: 20
vm_state: poweredon
