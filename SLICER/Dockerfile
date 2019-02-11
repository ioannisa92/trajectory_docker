# Use an official R image
FROM r-base

# Set the working directory to /slicer
WORKDIR /slicer

# Copy the src  contents into the container at /slicer
COPY src/ /slicer

# Install dependent packages for SLICER
RUN R -e "install.packages(c('SLICER', 'lle'),dependencies=TRUE, repos='http://cran.rstudio.com/')"

# Run test.R when the container launches
CMD ["Rscript", "SLICER_example.R"]
