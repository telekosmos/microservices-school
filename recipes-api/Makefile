SERVICE_PORT=3000

start:
	@docker run -d -p $(SERVICE_PORT):$(SERVICE_PORT) -e SERVICE_ENV=live -e MONGO_URL=$(MONGO_URL) -e RABBIT_PWD=$(RABBIT_PWD) -e SUMO_URL=$(SUMO_URL) --name $(SERVICE) --network=local $(SERVICE):$(TRAVIS_BUILD_NUMBER)

include ../Makefile
