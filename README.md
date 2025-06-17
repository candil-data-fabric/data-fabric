# CANDIL Data Fabric

This repository provides a Helm chart for deploying the CANDIL Data Fabric. The chart depends several other helm charts representing the components that comprise the Data Fabric.

## Prerequirements

- Kubernetes
- Helm

## Installation

### Using the Helm repository hosted in GitHub Pages

First, add the Helm repository:

```bash
$ helm repo add data-fabric https://candil-data-fabric.github.io/data-fabric/
```

Then, install the Helm Chart:

```bash
$ helm install data-fabric .
```

The chart will be installed using the default values. Use the provided [`values.yaml`](values.yaml) file in this repository as template to upgrade the installation with your desired parameters:

```bash
$ helm upgrade data-fabric -f myvalues.yaml
```

To uninstall the Helm Chart, run the following command:

```bash
$ helm uninstall data-fabric
```

### Cloning this repository

First, clone the repository:

```bash
$ git clone https://github.com/candil-data-fabric/data-fabric.git
```

Once cloned, edit the [`values.yaml`](values.yaml) file to match your deployment needs and run the following command:

```bash
$ helm install data-fabric .
```

To uninstall the Helm Chart, run the following command:

```bash
$ helm uninstall data-fabric
```
## Acknowledgements

This work was partially supported by the following projects:

- **UNICO 5G I+D 6G-DATADRIVEN**: Redes de próxima generación (B5G y 6G) impulsadas por datos para la fabricación sostenible y la respuesta a emergencias. Ministerio de Asuntos Económicos y Transformación Digital. European Union NextGenerationEU.

![UNICO](./images/ack-logo.png)
