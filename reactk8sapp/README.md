

### Build app locally
`yarn start` localhost:3000
`yarn test` Launches the test runner in the interactive watch mode.
`yarn build` Builds the app for production to the `build` folder.

## Create docker image of your app
Navigate to desired app directory with dockerfile:
`docker build -t <NAME> .`

Push the image to your dockerhub repo:
`docker push <DOCKERHUBUSER>/<REPONAME>:<TAG>`

Run a docker image of app:
`docker run -d -p <PORTF>:80 <APPNAME>`

## K8S
For minikube:
`minikube start`

For Docker Desktop User: Enable kubernetes in docker desktop to run a k8s cluster with a single node.

Navigate to pods directory with desired manifest yml. (pod.yml)
Make sure container image is correct dockerhub/repo.
`kubectl apply -f <manifest>`
