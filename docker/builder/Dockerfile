ARG CEPH_RELEASE=v15.2.4
FROM ceph/ceph:${CEPH_RELEASE}

RUN dnf group install -y 'Development Tools' && \
    dnf install -y cmake rados-objclass-devel && \
    dnf install -y --enablerepo=epel --enablerepo=PowerTools gtest-devel && \
    dnf clean all
