FROM continuumio/anaconda3

RUN conda install -c conda-forge -y gdal 
#RUN conda install -c conda-forge -y basemap
ENV PROJ_LIB=/opt/conda/share/proj
RUN pip install rasterio plotnine shapely circles geopandas folium GDAL

CMD jupyter-lab --ip=0.0.0.0 --no-browser --allow-root
