# mvapich2_spack

Install mvapich2 via spack on RHEL7

module purge

module load intel-18.0.1-gcc-8.1.0-rfzhv4x
spack install mvapich2 %intel



==> Executing phase: 'configure'
==> Error: ProcessError: Command exited with status 1:
    '/nv/ap5/usr-local-rhel7.4/pacerepov2/spack/var/spack/stage/mvapich2-2.2-4cy2ajbiylutcif7mdbn6wach47w7sud/mvapich2-2.2/configure' '--prefix=/nv/ap5/usr-local-rhel7.4/pacerepov2/spack/opt/spack/linux-rhel7-x86_64/intel-18.0.1/mvapich2-2.2-4cy2ajbiylutcif7mdbn6wach47w7sud' '--enable-shared' '--enable-romio' '--disable-silent-rules' '--disable-new-dtags' '--enable-fortran=all' '--enable-threads=multiple' '--with-ch3-rank-bits=32' 'CC=/nv/ap5/usr-local-rhel7.4/pacerepov2/spack/opt/spack/linux-rhel7-x86_64/gcc-4.8.5/intel-18.0.1-7cbw2rpdcuv3hpj2txc4wqcjnjeiv7n6/compilers_and_libraries_2018.1.163/linux/bin/intel64/icc' 'CXX=/nv/ap5/usr-local-rhel7.4/pacerepov2/spack/opt/spack/linux-rhel7-x86_64/gcc-4.8.5/intel-18.0.1-7cbw2rpdcuv3hpj2txc4wqcjnjeiv7n6/compilers_and_libraries_2018.1.163/linux/bin/intel64/icpc' 'FC=/nv/ap5/usr-local-rhel7.4/pacerepov2/spack/opt/spack/linux-rhel7-x86_64/gcc-4.8.5/intel-18.0.1-7cbw2rpdcuv3hpj2txc4wqcjnjeiv7n6/compilers_and_libraries_2018.1.163/linux/bin/intel64/ifort' 'F77=/nv/ap5/usr-local-rhel7.4/pacerepov2/spack/opt/spack/linux-rhel7-x86_64/gcc-4.8.5/intel-18.0.1-7cbw2rpdcuv3hpj2txc4wqcjnjeiv7n6/compilers_and_libraries_2018.1.163/linux/bin/intel64/ifort' '--disable-alloca' '--enable-fast=all' '--disable-cuda' '--enable-registration-cache' '--with-device=ch3:psm' '--with-psm=/nv/ap5/usr-local-rhel7.4/pacerepov2/spack/opt/spack/linux-rhel7-x86_64/intel-18.0.1/psm-3.3-3ppmjwgssklksgrwmgifvwtp3upz7b6y'

1 error found in build log:
     915    checking for sys/types.h... (cached) yes
     916    checking for errno.h... (cached) yes
     917    checking psm.h usability... yes
     918    checking psm.h presence... yes
     919    checking for psm.h... yes
     920    checking for psm_init in -lpsm_infinipath... no
  >> 921    configure: error: 'psm_infinipath library not found.  Did you specify --with-psm= or --with-psm-lib=?'
