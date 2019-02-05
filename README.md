# A Complete Guide to an Interactive Geographical Map using Python

Ever wondered how these beautiful geographical maps are created? Our World in Data has an extensive collection of interactive data visualizations on aspects dedicated to the global changes in health, population growth, education, culture, violence, political power, technology and several things that we care about. These visualizations help us understand how and why the world has changed over the last few decades. I was intrigued with this wealth of information and motivated to dive deeper.

[Blog]()

# Pre-requisites
- [Docker](https://docs.docker.com/install/)
- [Docker Compose](https://docs.docker.com/compose/install/)

# Directory Layout

```
.
├── Interactive-choropleth-map-obesity.mov
├── README.md
├── bokeh-app
│   ├── data
│   │   ├── countries_110m
│   │   │   ├── ne_110m_admin_0_countries.README.html
│   │   │   ├── ne_110m_admin_0_countries.VERSION.txt
│   │   │   ├── ne_110m_admin_0_countries.cpg
│   │   │   ├── ne_110m_admin_0_countries.dbf
│   │   │   ├── ne_110m_admin_0_countries.prj
│   │   │   ├── ne_110m_admin_0_countries.shp
│   │   │   └── ne_110m_admin_0_countries.shx
│   │   └── obesity.csv
│   └── world_obesity.ipynb
├── docker
│   └── Dockerfile
└── docker-compose.yml
```

# Running the sample

## Step 1 : Starting docker container

``` bash
$ git clone 
$ cd /root-dir-of-the-repository
$ docker-compose up
```
On the console output copy the jupyter notebook url e.g. `http://localhost:8888/token?=xxxx` and paste in your browser.

## Step 2 : Execute Code 

Open `world_obesity.ipynb` file and rull all cells.

## Step 3 : Start bokeh server

In the browser using the jupyter notebook go to the `Terminal` 

```
bokeh serve --show world_obesity.ipynb
```
## Step 4 : Browse the interactive map

The interactive map is rendered by bokeh server which can be browsed at `http://localhost:5006/`
