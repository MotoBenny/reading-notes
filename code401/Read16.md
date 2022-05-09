# [Serverless Computing](https://www.ibm.com/cloud/learn/serverless)

- Serverless is a cloud computing model that dynamically provisions computational power depending on the resources required to run the code.
- It automatically scales the resources depending on demand.

Offloads all backend responsibility (this is what I used to do, manage those servers/design them, and provision them based on load) to a cloud provider. A remote server management service, like AWS, Azure, Kubernettes.

Serverless computing, isnt serverless, Its just that someone else is managing the server.

### Pros
- Allows a development team to focus on the code, and the development therin, rather than managing infrastructure to run the code.
- Allows customers to pay only for the computational power they need, rather than to manage and maintain massive computational overhead.
- Serverless simplifies deployment


### Cons
- Serverless isnt generally as cost effective for stable workflows, If you have a very predicatble demand for your hardware, the adaptible, flexibility offered by serverless functions rarely benifits you.
- Based on demand and application serverless functions sometimes start cold, or from zero to serve a single function or request, downtime that is unacceptible depending on the application.
- It can complicate already complex processes of monitoring and debugging.
- And create locked in/inflexible dependancies in your systems, where you are beholden to a provider, like Docker, or VM.