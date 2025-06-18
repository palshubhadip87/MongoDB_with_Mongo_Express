# MongoDB with Mongo Express Sample Application
The purpose of this project to design a sample application with MongoDB and Mongo Express with persistent volume. This application may be used for any migration tests with persistent volume.

When request comes from browser, the OpenShift route will forward the traffic to Mongo Express service, which in turn forward it to Mongo Express POD. This POD is connected to Mongo DB service with a configmap and eventually traffic goes to Mongo DB POD. MongoDB deployed as a Statefulset application with persistent volume (PVC) from the Primary storage system. The MongoDB application is brought up on the secondary site with the replicated PVC from the secondary storage system. The sample application consists of the uploaded manifest files.
