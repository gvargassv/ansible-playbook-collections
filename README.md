# ⚙️ Ansible Playbook Collections

Colección de **playbooks de Ansible** para la automatización de tareas en entornos de **infraestructura TI**.  
Este repositorio está pensado como un espacio práctico para almacenar, compartir y reutilizar playbooks que resuelven necesidades reales de administración y operaciones.  

---

## 📌 Objetivo
El propósito de este repositorio es construir una **biblioteca simple y útil de playbooks** que puedan ayudar a:  
- Administradores de sistemas  
- Ingenieros de automatización  
- Profesionales DevOps  

Cada playbook es independiente y está enfocado en una tarea específica.  

---

## 🚀 Ejemplos de playbooks incluidos
- Gestión de usuarios y grupos  
- Despliegue de paquetes y parches  
- Configuración de servicios básicos  
- Monitoreo y validación de estado  
- Operaciones de mantenimiento de servidores  

*(La lista crecerá conforme se agreguen nuevos playbooks.)*  

---

## 📦 Requisitos
- **Ansible 2.9+** (recomendado: última versión estable)  
- Acceso SSH a los servidores de destino  
- Python instalado en los hosts gestionados  

---

## 🛠️ Uso básico
Ejecutar un playbook en modo simple:  

```bash
ansible-playbook playbook.yml -i inventario.ini
