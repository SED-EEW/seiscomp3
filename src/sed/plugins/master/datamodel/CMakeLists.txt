SET(PACKAGE_NAME DMPLUGINS)

SET(DMSM_SOURCES plugin_sm.cpp)
SET(DMVS_SOURCES plugin_vs.cpp)

SC_ADD_PLUGIN_LIBRARY(DMSM dmsm "")
SC_LINK_LIBRARIES_INTERNAL(dmsm datamodel_sm)

SC_ADD_PLUGIN_LIBRARY(DMVS dmvs "")
SC_LINK_LIBRARIES_INTERNAL(dmvs datamodel_vs)
