FROM ubuntu:18.04

RUN apt-get update
RUN apt-get install -y cups libcups2-dev libcupsimage2-dev gcc g++ automake git

COPY ./ /dymo
WORKDIR /dymo
RUN aclocal
RUN automake --add-missing
RUN autoconf
RUN ./configure
RUN make
RUN make install
 
CMD ["/bin/bash", "make"]