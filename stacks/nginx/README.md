# Nginx Stack

## Stacks

- docker and compose

## Guideline

This nginx compose use unprivilledge image to allow running without root
privilledges. To use this one we must before hand create networks as there are
many stacks and we do not know which stacks will be created first, so to
simplify the process we will create network via docker

```shel
docker network create {network_name}
```

## Configuration

Each website will define a site available configuration and put it in
`conf.d/site-availables`
