
FROM python:3.8

RUN apt-get update && apt-get install -y --no-install-recommends build-essential \
    python3-dev \ 
    llvm \ 
    llvm-dev
# Instal pytorch before rmbg !!
RUN pip3 install https://download.pytorch.org/whl/cpu/torch-1.7.1%2Bcpu-cp38-cp38-linux_x86_64.whl \
    https://download.pytorch.org/whl/cpu/torchvision-0.8.2%2Bcpu-cp38-cp38-linux_x86_64.whl
RUN pip3 install rembg
EXPOSE 5000
ENTRYPOINT ["rembg-server"]
CMD []