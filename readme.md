# Tutorial 

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