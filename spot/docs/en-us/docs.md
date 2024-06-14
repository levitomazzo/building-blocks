## Spot

️Folder Structures

>:open_file_folder: src
>
>> :open_file_folder: layers :mortar_board: This folder is used to store the list of layers.
>>> :page_facing_up: layers.go :heavy_exclamation_mark: This file is crucial. Refer to the [detailed documentation](./../../templates/src/layers/README.md) for more information.
>>
>> :open_file_folder: proto
>>
>> :open_file_folder: proto-gen :mortar_board: It contains files generated based on the proto files.
>>
>> :open_file_folder: servers
>>
>>> :open_file_folder: health 
>>>> :open_file_folder: v1
>>>>> :page_facing_up: healthServer.go :mortar_board: Server gRPC for Health Checking
>>>>
>>> :open_file_folder: spot 
>>>> :open_file_folder: v1
>>>>> :page_facing_up: spot.go :mortar_board: Server gRPC for Spot
>>>>
>>>
>>
> :page_facing_up: .clang-format :mortar_board: Format proto files
>
> :page_facing_up: go.mod :mortar_board: The package management file.
>
> :page_facing_up: go.sum :mortar_board: The file used by the package manager.
>
> :page_facing_up: maing.go :mortar_board: Entry point of the application.
>
> :page_facing_up: Makefile
>
> :page_facing_up: stackspot.yaml

## Requirements

### :wrench: Tools and technologies

| Name | Documentation |
|----------|----------|
| Go  |[link](https://go.dev/doc/install) |
| Rancher Desktop  |[link](https://docs.rancherdesktop.io/getting-started/installation/) |
| Protocol Buffer Compiler  |[link](https://grpc.io/docs/protoc-installation/) |
| Protoc Go Inject Tag  |[link](https://github.com/favadi/protoc-go-inject-tag) |
| grpcurl |[link](https://github.com/fullstorydev/grpcurl) |
| Make | - |


#### For Linux Ubuntu

| Install  - make

```shell
sudo apt install make
```

### :electric_plug: VS Code  Plugins

| Name | Source |
|----------|----------|
| StackSpot AI| [link](https://marketplace.visualstudio.com/items?itemName=StackspotAI.StackSpotAI)|
| Proto 3 |[link](https://marketplace.visualstudio.com/items?itemName=zxh404.vscode-proto3) |
| Yaml |[link](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml) |
| Go|[link](https://marketplace.visualstudio.com/items?itemName=golang.Go) |
| Clang-Format | [link](https://marketplace.visualstudio.com/items?itemName=xaver.clang-format) |
| Docker  | [link](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)  |
| Makefile Tools| [link](https://marketplace.visualstudio.com/items?itemName=ms-vscode.makefile-tools)|
| Markdown Emoji | [link](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-emoji)|
| Material Icon Theme | [link](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)|


## Usage


## Release Notes
