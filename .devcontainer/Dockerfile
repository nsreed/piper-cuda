ARG VARIANT="ubuntu20.04" 
ARG CUDA_VERSION="12.1.1"
FROM nvidia/cuda:${CUDA_VERSION}-devel-${VARIANT}


# [Optional] Uncomment this section to install additional OS packages.
# RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
#     && apt-get -y install --no-install-recommends <your-package-list-here>

# RUN apt-get update && apt-get install -y python3-opencv
# RUN apt-get update && apt-get install -y pip
# RUN python3 -m pip install --no-cache -r requirements.txt

RUN apt-get update && apt-get install -y wget
#conda???
# USER vscode
# Download installer https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
# RUN wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
# RUN bash Miniconda3-latest-Linux-x86_64.sh -b


RUN wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O /opt/miniconda.sh
RUN bash /opt/miniconda.sh -b -p /opt/miniconda
RUN /opt/miniconda/bin/conda init --all