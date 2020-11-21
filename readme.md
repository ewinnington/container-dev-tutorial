# Tutorial 

This is a repository containing a collection of the devcontainers used for the polyglot poject. Each subfolder can be opened in visual studio code as a developer container. Here, no code is committed, only the container configuration itself.

Following <https://docs.microsoft.com/en-gb/learn/modules/use-docker-container-dev-env-vs-code/1-introduction>

The devcontainer images are available at https://hub.docker.com/_/microsoft-vscode-devcontainers 

F1 to open the VSCode menu then "Remote Container: Add Development container configuration"

## Python

The Python devcontainer works.  

## DotNet 

Works with dotnet core 3.1, dotnet 5.0 is not currently in the devcontainers. 

dotnet new console

## Rust

cargo init
cargo run

## Go

go run

## Java

mvn archetype:generate -DgroupId=com.cloudplush.hw -DartifactId=my-hw -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false

cd my-hw mvn package

java -cp target/my-hw-1.0-SNAPSHOT.jar com.cloudplush.hw.App

## Swift

The devcontainer was changed from the default due to an error message in the api-get update command. 

swift package init --type executable

## Typescript 

npm init
npm install -D typescript@3.3.3
npm install -D tslint@5.12.1

tsc --init 

touch index.ts
tsc
node index.js 

## Cpp

The devcontainer was changed from the default due to an error message in the api-get update command. 

The CPP development container is configured to use vcpk for the dependencies.
