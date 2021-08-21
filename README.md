# Cloud Abstractor

**A set of .NET libraries that make your application portable between clouds (Azure, AWS, GKE, even on-premises) by providing a common abstraction layer over services that are specific to a particular provider.**

## The Motivation

In the world of microservices hosted in containers, one of the commonly mentioned benefits is the ability to move such an application between various cloud providers and even on/off-premises. While this is true to an extent, in the real world the portability is hindered by the fact that such applications typically use external dependencies such (queues, storages etc.), which are vendor specific.

E.g., you can’t switch from *Azure Blob storage* to *AWS S3* just by changing the connection string although both are fundamentally very similar.
This project aims to remove such vendor lock-ins by providing a common abstraction layer over the services.
