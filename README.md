# activeMQ
Apache ActiveMQ™ is the most popular open source, multi-protocol, Java-based messaging server. It supports industry standard protocols so users get the benefits of client choices across a broad range of languages and platforms. Connectivity from C, C++, Python, .Net, and more is available. Integrate your multi-platform applications using the ubiquitous AMQP protocol. Exchange messages between your web applications using STOMP over websockets. Manage your IoT devices using MQTT. Support your existing JMS infrastructure and beyond. ActiveMQ offers the power and flexibility to support any messaging use-case.
There are currently two "flavors" of ActiveMQ available - the "classic" 5.x broker and the "next generation" Artemis broker. Once Artemis reaches a sufficient level of feature parity with the 5.x code-base it will become ActiveMQ 6. Initial migration documentation is available.
This document will walk through the basic flavour of ActiveMQ classic broker.

Installtions through Helm charts
create namespace required name space if any

kubectl create namespace {namespace}


Install helm chart attached:

helm install activemq  --name activemq --namespace {namespace}
Check the pods are deployed for activeMQ:

kubectl get pods -n {namespace}
kubectl get svc -n {namespace} | grep activemq
On successful deployment check the activemq GUI from bellow command:

use default credentials as admin/admin 

{Masterip}:30742
