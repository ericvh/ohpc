# ARM64 Version of CentOS OpenHPC build
# http://openhpc.community
#
# VERSION               0.0.1

FROM multiarch/centos:aarch64-clean
MAINTAINER Eric Van Hensbergen <ericvh@gmail.com>
RUN yum -y update && yum -y install http://build.openhpc.community/OpenHPC:/1.3/CentOS_7/aarch64/ohpc-release-1.3-1.el7.aarch64.rpm && yum -y install ohpc-base && yum -y install ohpc-warewulf && yum -y install ohpc-autotools EasyBuild-ohpc hwloc-ohpc spack-ohpc valgrind-ohpc gnu7-compilers-ohpc llvm4-compilers-ohpc openmpi-gnu7-ohpc ohpc-gnu7-perf-tools lmod-defaults-gnu7-openmpi-ohpc ohpc-gnu7-serial-libs ohpc-gnu7-io-libs ohpc-gnu7-python-libs ohpc-gnu7-runtimes ohpc-gnu7-openmpi-parallel-libs && yum clean all
WORKDIR /root
ENTRYPOINT ["bash", "-i"]
