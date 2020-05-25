From alpine
RUN apk add libstdc++ && apk add icu && apk add libintl
RUN wget https://download.visualstudio.microsoft.com/download/pr/5f4e2183-6e50-4334-bdf7-3c2944c6d023/724b9946eaa705ee776fe3c1f68918f0/dotnet-sdk-3.1.201-linux-musl-x64.tar.gz
RUN mkdir -p $HOME/dotnet && tar zxf dotnet-sdk-3.1.201-linux-musl-x64.tar.gz -C $HOME/dotnet
RUN rm /dotnet-sdk-3.1.201-linux-musl-x64.tar.gz
ENV DOTNET_ROOT /root/dotnet
ENV PATH $PATH:/root/dotnet
WORKDIR /data
