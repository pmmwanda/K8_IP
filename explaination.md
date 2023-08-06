Choice of Objects Used
This project utilizes deployment, services, config maps, and persistent volume. The files are separated into the backend and the client directory for efficiency.

The services for both client and backend are set to ensure that they are exposed externally.

Storage solutions
For the MongoDB database, to ensure persistent storage for data integrity it will use Kubernetes PersistentVolume (PV) and PersistentVolumeClaim (PVC). The PersistentVolume is a cluster-wide resource that represents a physical storage device, while the PersistentVolumeClaim is a request for storage by a pod. The PVC binds to the PV, providing a reliable storage solution for MongoDB data.

Git workflow
The K8 files are version-controlled using Git alongside other project files, and changes are be committed and pushed to a Git repository.