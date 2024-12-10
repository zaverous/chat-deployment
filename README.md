# Despliegue de la Aplicación CIMSI Chat

Este proyecto despliega la aplicación **CIMSI Chat** en un clúster de Kubernetes utilizando los recursos definidos en la rama `deploy`. La aplicación está compuesta por tres componentes principales: **Frontend**, **Backend** y **MongoDB**.

---

## **Requisitos Previos**

Antes de realizar la instalación, asegúrate de que tu entorno cumple con los siguientes requisitos:

1. **Kubernetes Clúster**:
   - Necesitas un clúster de Kubernetes listo para usar. En este caso, se utilizó Minikube, pero puedes usar cualquier proveedor compatible con Kubernetes.

2. **Kubectl**:
   - Herramienta de línea de comandos para interactuar con el clúster.
   - [Instrucciones de instalación de `kubectl`](https://kubernetes.io/docs/tasks/tools/install-kubectl/).

3. **Docker**:
   - Asegúrate de tener Docker instalado y configurado en tu máquina.
   - [Instrucciones de instalación de Docker](https://docs.docker.com/get-docker/).

4. **ArgoCD (Opcional)**:
   - Si usas ArgoCD para monitorear el despliegue, asegúrate de que esté instalado y configurado.

---

## **Instalación**

El proceso de instalación de la aplicación es muy sencillo. Solo necesitas ejecutar el siguiente comando para desplegar todos los recursos en tu clúster:

```bash
kubectl apply -f "https://github.com/zaverous/chat-deployment/blob/deploy/aplicacion.yaml"