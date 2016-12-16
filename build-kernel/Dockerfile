FROM fedora:rawhide

MAINTAINER Alexander Alemayhu

RUN dnf update -y
RUN dnf install -y git kernel-devel gcc elfutils-libelf-devel
RUN dnf install -y 'dnf-command(builddep)'
RUN dnf builddep -y kernel
RUN dnf clean all

RUN git clone git://git.kernel.org/pub/scm/linux/kernel/git/davem/net.git
