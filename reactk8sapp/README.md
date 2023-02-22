

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

## Containerizing

For minikube:
run 'minikube start'

For Docker Desktop User: Enable kubernetes in docker desktop to run a k8s cluster with a single node.

## create docker image of your app
Navigate to desired app directory with dockerfile:
run 'docker build -t <NAME> .'

Push the image to your dockerhub repo:
run 'docker push <DOCKERHUBUSER>/<REPONAME>:<TAG>'

Run a docker image of app:
run 'docker run -d -p <PORTF>:80 <APPNAME>

## To create k8s pod/service/deployment with your app
Navigate to pods directory with desired manifest yml. (pod.yml)
Make sure container image is correct dockerhub/repo.
run 'kubectl apply -f <manifest>'
