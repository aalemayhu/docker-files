project=scanf/build-kernel

docker:
	docker build -t ${project} .
docker-deploy: docker push_hub
	echo "Pushed to docker"
docker-run: docker
	docker run -t -i ${project} /bin/bash
docker-push:
	docker push ${project}
