# phpadr-dockerized

This image help you to use [globtec/phpadr](https://github.com/globtec/phpadr) in any tech stack.

## How to use this image

Starting with PHPADR Tools is simple, execute the following command:
```
docker run -it --rm --user $(id -u):$(id -g) --volume $PWD:/workspace rafaelsobreirabraga/phpadr-dockerized [arguments] [options]
```

Do you can create `phpadr.sh` shell file with the statement above for simplefy, after do you can use:
```
./phpadr.sh command [arguments] [options]
```

For example, to create a new ADR 
```
./phpadr.sh make:decision <title> [<status="Accepted">] [--directory="docs/arch"]
```

## Help

For more help execute the following command:
```
./phpadr.sh <command> --help
```