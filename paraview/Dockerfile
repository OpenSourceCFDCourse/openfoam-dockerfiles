FROM openfoam:2112

USER root

# install paraview
RUN apt-get update && apt-get install -y --no-install-recommends \
    paraview

# do some cleaning up
RUN apt-get clean && rm -rf /var/lib/apt/lists/*

# switch back to user foam
USER foam