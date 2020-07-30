.PHONY: build install

pandoc_image = pandoc/latex:latest

pandoc_command = docker run \
				 --interactive \
				 --tty \
				 --rm \
				 --volume "$(shell pwd):/data" \
				 --volume "$(shell pwd)/fonts:/root/.fonts" \
				 $(pandoc_image) \
				 --defaults=config/defaults.yaml \
				 --metadata-file=config/metadata.yaml \

build:
	$(call pandoc_command)

install:
	docker pull $(pandoc_image)
