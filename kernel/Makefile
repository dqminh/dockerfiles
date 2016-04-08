.PHONY: build
build:
	docker build -t dqminh/kernel .

.PHONY: run
run: build
	docker run -it -v $(PWD):/root dqminh/kernel bash

.PHONY: push
push: build
	docker push dqminh/kernel
