# worm-notebooks


## Notes on setting up cellxgenes on AWS EC2 instance
https://chanzuckerberg.github.io/cellxgene/


```
sudo apt update
sudo apt install python3
sudo apt install python3-pip

```
Installing anaconda.. because cellxgenes pip install is broken
https://www.digitalocean.com/community/tutorials/how-to-install-anaconda-on-ubuntu-18-04-quickstart
```
wget https://repo.anaconda.com/archive/Anaconda3-2020.02-Linux-x86_64.sh
bash Anaconda3-2020.02-Linux-x86_64.sh

cd ~
source .bashrc
conda list ## this verifies the installation
```

Now in the conda python 3.7 environment we can do:
https://chanzuckerberg.github.io/cellxgene/posts/launch
```
pip install cellxgene


cellxgene launch CPT_wormcells_embeddings.h5ad --open --disable-diffexp --about https://de.wormcells.com/ --title "Visualizing C. elegans single cell data. Visit de.wormcells.com to learn about the datasets" --host 0.0.0.0 --port 8080



```






