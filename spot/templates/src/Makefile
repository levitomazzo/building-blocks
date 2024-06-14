start:
	make -s -f Makefile.spot start

list-server:
	make -s -f Makefile.spot list-server

health:
	make -s -f Makefile.spot health

list-spot-rpc:
	make -s -f Makefile.spot list-spot-rpc

list-layers:
	make -s -f Makefile.spot list-layers

call:
	make -s -f Makefile.spot call

go-run-binary:
	PLAYGROUND=enable \
	HOST=0.0.0.0 \
	PORT=50051 \
	REFLECTION=enable \
	./spot

go-build:
	GOOS=linux GOARCH=amd64 go build .
	# GOOS=darwin GOARCH=amd64 go build .

rm-generated:
	mkdir -p proto-gen 
	rm -rf proto-gen/*

generated: rm-generated
	protoc \
		--go_out=./proto-gen \
		--go-grpc_out=./proto-gen \
		 proto/*/*/*.proto

proto: generated
	protoc-go-inject-tag -input="proto-gen/*/*.pb.go" -remove_tag_comment

.SILENT: