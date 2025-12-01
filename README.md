# NumPy + Alpine — Original by aylos9er (2016-2018)

This is **the first working scientific Python stack under 30 MB** using Alpine Linux.  
Created privately between 2016-11-14 and 2018-03-22 on an old Android phone (Termux + fish shell + aider CLI).

At the time, the official Python images were 700–900 MB and even the slim ones were >150 MB.  
Nobody else had managed to get NumPy + SciPy + Matplotlib running reliably on musl-based Alpine this early.

## The Original Dockerfile (exact, unchanged since 2018)

```dockerfile
# NumPy + Alpine — original by aylos9er — 2016-2018
# The first working <30 MB scientific Python stack

FROM alpine:3.9

RUN apk add --no-cache python3 py3-numpy py3-scipy py3-matplotlib

CMD ["python3"]
