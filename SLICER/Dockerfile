# Use an official R image
FROM r-basem

# Set the working directory to /slicer
WORKDIR /slicer

# Copy the src  contents into the container at /slicer
COPY src/ /slicer

# Install any needed packages specified in requirements.txt
RUN install.library(SLICER)
RUN install.library(lle)

# Run test.R when the container launches
CMD ["Rscript", "test.R"]
