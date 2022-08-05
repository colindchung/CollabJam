# CollabJam

From concert bands to aspiring SoundCloud rappers, people often work with others to create music. However, groups lack the ability to edit audio together in real time and often resort to sending audio files back and forth. CollabJam enables musicians to create their music collaboratively by providing a single web interface where they can upload, edit and share their music while receiving real-time updates from others on their team.

## Design
### Concurrency Control
One of the primary challenges for this project is concurrency control among users making parallel edits to the same properties of audio clips. At a high level, this is reconciled using a conflict-free replicated data type (CRDT) updated with last-write wins (LWW) semantics. Bidirectional communication between active clients and the server is handled using web sockets.


## Technologies and tools
Listed below are some of the tools and technologies that were used in constructing this product.

### Frontend
- [React.js](https://reactjs.org/)
- [Web Audio API](https://www.w3.org/TR/webaudio/)
- [Wavesurfer.js](https://wavesurfer-js.org/)
- [CloudConvert](https://cloudconvert.com/)
- [Wix](https://www.wix.com/) (for mockups)

### Backend
- [Golang](https://go.dev/)
- [MySQL](https://www.mysql.com/)
- [Docker](https://www.docker.com/)
- [dbdiagram.io](https://dbdiagram.io/home)

### Infrastructure
- [Amazon Web Services](https://aws.amazon.com/)
	- Simple Storage Service (S3)
	- Relational Database Service (RDS)
	- Elastic Container Service (ECS)
	- Elastic Container Registry (ECR)
	- Elastic Compute Cloud (EC2)
	- Secrets Manager
	- Route53
	- AWS Certificate Manager (ACM)
- [Docker](https://www.docker.com/)
- [Netlify](https://www.netlify.com/)
