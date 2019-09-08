all: image push server client

image:
	docker build -t functicons/hello-k8s .

push: image
	docker push functicons/hello-k8s

server:
	kubectl apply -f server.yaml

client:
	kubectl apply -f client.yaml