ENABLE_LANGUAGE(Fortran)
SET(CMAKE_Fortran_FLAGS "-O3 -Wsurprising -I. -g -std=legacy")
INCLUDE_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR})
SET(URQMD_CORSIKA_SRC addpart.f angdis.f anndec.f blockres.f boxprg.f cascinit.f coload.f dectim.f delpart.f detbal.f dwidth.f error.f getmass.f getspin.f init.f  iso.f ityp2pdg.f jdecay2.f make22.f numrec.f output.f paulibl.f proppot.f saveinfo.f scatter.f siglookup.f string.f tabinit.f urqmd.f whichres.f)
ADD_LIBRARY(URQMD_CORSIKA STATIC ${URQMD_CORSIKA_SRC})