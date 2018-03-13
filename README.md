# phpadr-dockerized

This container help you to use [globtec/phpadr](https://github.com/globtec/phpadr) in any tech stack.

## How to use this image

Starting with PHPADR Tools is simple, execute the following command:

```
docker run -it --rm --user $(id -u):$(id -g) --volume $PWD:/workspace rafaelsobreirabraga/phpadr-dockerized "$@"
```

Do you can create `phpadr.sh` shell file with the statement above for simplefy, after do you can use:

```
./phpadr command [arguments] [options]
```

For example, to create a new ADR 
```
./phpadr make:decision <title> [<status="Accepted">] [--directory="docs/arch"]
```

## Help

For more hel execute the following command:
```
./phpadr <command> --help
```