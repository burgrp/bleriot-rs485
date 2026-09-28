INSTANCE ?= em.grid

.PHONY: build flash gdb rtt install-pack disassembly new hub

build:
	go run ./cmd/dev node build --name $(INSTANCE)

flash:
	go run ./cmd/dev node build --name $(INSTANCE) --flash --rtt

disassembly:
	go run ./cmd/dev node build --name $(INSTANCE) --disassembly

gdb rtt install-pack:
	go run ./cmd/dev node $@ --name $(INSTANCE)

new:
	go run ./cmd/dev node new

hub:
	go run ./cmd/dev hub --diagnostics rf