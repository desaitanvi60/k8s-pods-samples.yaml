
🌟 Kubernetes YAML Files Overview

This repository contains various YAML configuration files for Kubernetes pods, each demonstrating different features and functionalities. Below is a brief explanation of each file.

1. configmap-pod.yaml📜
This file defines a Kubernetes ConfigMap that stores configuration data for applications.A ConfigMap allows you to decouple environment-specific configurations from your container images, helping you manage configurations separately and enabling easy updates without rebuilding your application.

  Key Features:
- 🔑 Defines key-value pairs that can be referenced in pods.
- 🛠️ Helps in providing configuration settings without hardcoding them into the application.

 2. env-pod.yaml🌍
This YAML file demonstrates how to use environment variables in a pod.Environment variables allow you to pass dynamic configuration values to your containers, which can be accessed by theapplications running inside the pods.

  Key Features:
- 🌱 Shows how to set environment variables directly in the pod specification.
- 🔄 Allows applications to adapt based on the environment they are running in (e.g., development, testing, production)

 3. multicontainerpod.yaml🚀
This file defines a multi-container pod where multiple containers run within the same pod.Multi-container pods are useful for closely related applications that need to work together.

  Key Features:
- 🔗 Configures multiple containers sharing the same network namespace.
- 📡 Enables inter-container communication, making it easier to manage dependent services.

 4. pod.yaml🐳
This is a basic configuration file for creating a single container pod in Kubernetes.It specifies the container image, name, and other essential parameters required to run a single application.

  Key Features:
- ⚙️ Defines a simple pod structure with a single container.
- 📦 Basic parameters such as `image`, `name`, and `ports` to expose the application.

 5. resource-limits-pod.yaml⏳
This file illustrates how to set resource requests and limits for a pod's containers.Resource limits ensure that your applications use only the specified amount of CPU and memory, which helps in managing cluster resources efficiently.

  Key Features:
- 📊 Specifies `requests` and `limits` for CPU and memory.
- 📈 Helps in optimizing resource allocation and ensuring fair usage among pods.

 6. secret-pod.yaml 🔒
This YAML file showcases how to use Secrets in Kubernetes to manage sensitive information, such as passwords, tokens, or keys. Secrets ensure that sensitive data is kept secure and is onlyaccessible to the necessary components.

  Key Features:
- 🛡️ Defines a Secret that can be mounted as an environment variable or volume in a pod.
- 🔑 Protects sensitive data by encoding it in base64.

7. security-context-pod.yaml ⚔️
This file defines a security context for a pod, which allows you to specify security attributes for the containers. Security contexts can control user IDs, privileges, and capabilities, enhancing the security of your applications.

  Key Features:
- 🚷 Configures settings such as running the container as a non-root user.
- ⚙️ Adds security options like `privileged` or `capabilities`

8. volume-pod.yaml📂
This YAML file demonstrates how to define and use volumes in a pod. Volumes provide persistent storage that can be shared between containers in a pod, ensuring data remains accessible across container restarts.

  Key Features:
- 🗃️ Specifies a volume type (e.g., `hostPath`, `emptyDir`, etc.).
- 🗄️ Shows how to mount the volume to a specific path inside the container.

Conclusion 🎉

Each of these YAML files provides essential configurations to manage and deploy applications in a Kubernetes cluster effectively. Feel free to explore each file and modify them according to your application's needs.

