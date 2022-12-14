# ullswater-stack

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.16.0](https://img.shields.io/badge/AppVersion-1.16.0-informational?style=flat-square)

A Helm chart for provisioning an Ullswater Stack

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| kafka.chartName | string | `"kafka"` |  |
| kafka.enabled | bool | `false` |  |
| kafka.helmValues | string | `"commonLabels: {}\ndiagnosticMode.enabled: false\n"` |  |
| kafka.namespace | string | `"kafka"` |  |
| kafka.repoURL | string | `"https://charts.bitnami.com/bitnami"` |  |
| kafka.targetRevision | string | `"19.1.3"` |  |
| minio.chartName | string | `"minio"` |  |
| minio.enabled | bool | `false` |  |
| minio.helmValues | string | `"tls.enabled: false\n"` |  |
| minio.namespace | string | `"minio"` |  |
| minio.repoURL | string | `"https://charts.bitnami.com/bitnami"` |  |
| minio.targetRevision | string | `"2.3.1"` |  |
| minioOperator.chartName | string | `"minio-operator"` |  |
| minioOperator.enabled | bool | `true` |  |
| minioOperator.helmValues | string | `""` |  |
| minioOperator.namespace | string | `"minio-operator"` |  |
| minioOperator.repoURL | string | `"https://operator.min.io/"` |  |
| minioOperator.targetRevision | string | `"4.3.7"` |  |
| postgresql.chartName | string | `"postgresql"` |  |
| postgresql.enabled | bool | `true` |  |
| postgresql.helmValues | string | `""` |  |
| postgresql.namespace | string | `"postgresql"` |  |
| postgresql.repoURL | string | `"https://charts.bitnami.com/bitnami"` |  |
| postgresql.targetRevision | string | `"12.1.2"` |  |
| senzingOperator.chartPath | string | `"senzing-chart/szchart"` |  |
| senzingOperator.enabled | bool | `false` |  |
| senzingOperator.helmValues | string | `""` |  |
| senzingOperator.namespace | string | `"senzing-operator"` |  |
| senzingOperator.repoURL | string | `"https://gitlab.com/dataedgeanalytics/ullswater/senzing-operator"` |  |
| senzingOperator.targetRevision | int | `20220316` |  |
| senzingStack.components[0].chartName | string | `"senzing-console"` |  |
| senzingStack.components[0].enabled | bool | `true` |  |
| senzingStack.components[0].helmValues | string | `""` |  |
| senzingStack.components[0].targetRevision | string | `"2.3.1"` |  |
| senzingStack.components[1].chartName | string | `"senzing-api-server"` |  |
| senzingStack.components[1].enabled | bool | `false` |  |
| senzingStack.components[1].helmValues | string | `""` |  |
| senzingStack.components[1].targetRevision | string | `"2.4.2"` |  |
| senzingStack.components[2].chartName | string | `"senzing-stream-loader"` |  |
| senzingStack.components[2].enabled | bool | `false` |  |
| senzingStack.components[2].helmValues | string | `""` |  |
| senzingStack.components[2].targetRevision | string | `"2.4.3"` |  |
| senzingStack.components[3].chartName | string | `"senzing-redoer"` |  |
| senzingStack.components[3].enabled | bool | `false` |  |
| senzingStack.components[3].helmValues | string | `""` |  |
| senzingStack.components[3].targetRevision | string | `"2.4.2"` |  |
| senzingStack.components[4].chartName | string | `"swaggerapi-swagger-ui"` |  |
| senzingStack.components[4].enabled | bool | `true` |  |
| senzingStack.components[4].helmValues | string | `""` |  |
| senzingStack.components[4].targetRevision | string | `"2.3.0"` |  |
| senzingStack.components[5].chartName | string | `"senzing-debug"` |  |
| senzingStack.components[5].enabled | bool | `true` |  |
| senzingStack.components[5].helmValues | string | `""` |  |
| senzingStack.components[5].targetRevision | string | `"1.3.0"` |  |
| senzingStack.components[6].chartName | string | `"senzing-init-postgresql"` |  |
| senzingStack.components[6].enabled | bool | `false` |  |
| senzingStack.components[6].helmValues | string | `""` |  |
| senzingStack.components[6].targetRevision | string | `"1.0.0"` |  |
| senzingStack.components[7].chartName | string | `"senzing-postgresql-client"` |  |
| senzingStack.components[7].enabled | bool | `false` |  |
| senzingStack.components[7].helmValues | string | `""` |  |
| senzingStack.components[7].targetRevision | string | `"2.2.0"` |  |
| senzingStack.enabled | bool | `false` |  |
| senzingStack.namespace | string | `"senzing"` |  |
| senzingStack.repoURL | string | `"https://hub.senzing.com/charts"` |  |
| spark.chartName | string | `"spark"` |  |
| spark.enabled | bool | `false` |  |
| spark.helmValues | string | `""` |  |
| spark.namespace | string | `"spark"` |  |
| spark.repoURL | string | `"https://charts.bitnami.com/bitnami"` |  |
| spark.targetRevision | string | `"6.3.11"` |  |
| sparkOperator.chartName | string | `"spark-operator"` |  |
| sparkOperator.enabled | bool | `true` |  |
| sparkOperator.helmValues | string | `""` |  |
| sparkOperator.namespace | string | `"spark-operator"` |  |
| sparkOperator.repoURL | string | `"https://googlecloudplatform.github.io/spark-on-k8s-operator"` |  |
| sparkOperator.targetRevision | string | `"1.1.26"` |  |
| strimziKafkaOperator.chartName | string | `"strimzi-kafka-operator"` |  |
| strimziKafkaOperator.enabled | bool | `true` |  |
| strimziKafkaOperator.helmValues | string | `""` |  |
| strimziKafkaOperator.namespace | string | `"strimzi-kafka-operator"` |  |
| strimziKafkaOperator.repoURL | string | `"https://strimzi.io/charts/"` |  |
| strimziKafkaOperator.targetRevision | string | `"0.32.0"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)
