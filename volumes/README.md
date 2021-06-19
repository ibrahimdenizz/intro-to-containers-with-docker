# Volumes

```
docker run --env <var-name>=<value> --mount type=volume,src=<source-path>,target=<target-path> <image-name> 
```
for this example

```
docker run --env DATA_PATH=/data/num.txt --mount type=volume,src=incrementor-data,target=/data incrementor
```