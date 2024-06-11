FROM mcr.microsoft.com/devcontainers/dotnet:8.0

RUN apt-get update && apt-get install -y \
  build-essential \
  scons \
  pkg-config \
  libx11-dev \
  libxcursor-dev \
  libxinerama-dev \
  libgl1-mesa-dev \
  libglu1-mesa-dev \
  libasound2-dev \
  libpulse-dev \
  libudev-dev \
  libxi-dev \
  libxrandr-dev

RUN git clone https://github.com/godotengine/godot.git
WORKDIR "godot"
RUN scons platform=linuxbsd target=editor
RUN ln /godot/bin/godot.linuxbsd.editor.x86_64 /bin/godot -s

ENV SHELL /bin/bash
