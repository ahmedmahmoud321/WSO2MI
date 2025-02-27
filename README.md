# WSO2MI

WSO2 Micro Integrator is a lightweight, cloud-native, and decentralized integration platform that allows you to
integrate services, systems, and data sources. It is based on the popular open-source project Apache Synapse. WSO2 Micro
Integrator is a cloud-native, lightweight, and decentralized integration platform that allows you to integrate services,
systems, and data sources. It is based on the popular open-source project Apache Synapse. WSO2 Micro Integrator is a
cloud-native, lightweight, and decentralized integration platform that allows you to integrate services, systems, and
data sources. It is based on the popular open-source project Apache Synapse.

### Topics

* [Message Routing](#message-routing)
* [Message Transformation](#message-transformation)
* [Message Processing](#message-processing)
* [Service Orchestration](#service-orchestration)
* [Asynchronous Messaging Processing](#asynchronous-messaging-processing)
* [Protocol Switching](#protocol-switching)
* [SaaS and B2B Integration](#saas-and-b2b-integration)
* [Data Integration](#data-integration)
* [File Processing](#file-processing)
* [Periodic Execution](#periodic-execution)
* [Rest API](#rest-api)
* [Websocket](#websocket)
* [Webhook](#webhook)
* [Proxy Service](#proxy-service)
* [Inbound Endpoint](#inbound-endpoint)
* [Local Entry](#local-entry)
* [Template](#template)
* [Message Store](#message-store)
* [Message Processor](#message-processor)
* [Endpoint](#endpoint)
* [Sequence](#sequence)

### Message Transformation

* Transform the message from one format to another format.

**From**

```json
{
  "name": "John Doe",
  "dob": "1940-03-19",
  "ssn": "234-23-525",
  "address": "California",
  "phone": "8770586755",
  "email": "johndoe@gmail.com",
  "doctor": "thomas collins",
  "hospital_id": "grandoaks",
  "hospital": "grand oak community hospital",
  "cardNo": "7844481124110331",
  "appointment_date": "2017-04-02"
}
```

**To**

```json
{
  "patient": {
    "name": "John Doe",
    "dob": "1990-03-19",
    "ssn": "234-23-525",
    "address": "California",
    "phone": "8770586755",
    "email": "johndoe@gmail.com",
    "cardNo": "7844481124110331"
  },
  "doctor": "thomas collins",
  "hospital_id": "grandoaks",
  "hospital": "grand oak community hospital",
  "appointment_date": "2017-04-02"
}
```

