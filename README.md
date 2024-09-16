## How to compile a paper ##
- Step 1: Clone this repository
```bash
git clone git@github.com:SalomePlatform/joss.git
```
- Step 2: Get all dependencies 
```bash
cd joss_papers
git submodule update --init --recursive
```

Finally to compile the pdf you have two options 

- Step 3.1: Compile with docker image 
```bash
cd salome
sudo docker run --rm -it \
    -v $PWD:/data \
    -u $(id -u):$(id -g) \
    openjournals/inara \
    -o pdf,crossref \
    ./paper.md
```

- Step 3.2: Compile with Latex via Makefile
```bash
cd inara
make pdf ARTICLE=./../salome/paper.md
```
The generated pdf will be written to folder `inara/publishing-artifacts`.
