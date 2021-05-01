# Inventory Management

Inventory Management is a headless inventory management platform built on Node.js, React.js and Kubernetes.

## Getting Started

Follow the steps below to initialize the development platform on your local system.

### Software Dependencies

- [Node.js](https://nodejs.org/)
- [Yarn](https://yarnpkg.com/)
- [Docker](https://docker.com/)
- [Kubernetes](https://kubernetes.io/)
- [Ingress NGINX](https://kubernetes.github.io/ingress-nginx/)
- [Skaffold](https://skaffold.dev)

### Setting up the Development Platform

Clone the repository in your local machine.

```sh
git clone https://github.com/benzene-tech/inventory-management.git
```

Run the setup file to install all the micro-services.

```sh
cd inventory-management && bash setup
```

This command will check for any missing software dependencies and will pull the latest Docker Images of the micro-services.

Once the script is executed without any errors, add the DNS inventory-management.com to your hosts file. This will require a super-user.

```sh
sudo vim /etc/hosts
```

Append the below snippet to the file.

```
127.0.0.1 inventory-management.com
```

Run the development cluster with

```sh
skaffold dev
```
