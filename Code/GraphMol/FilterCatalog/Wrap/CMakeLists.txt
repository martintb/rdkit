rdkit_python_extension(rdfiltercatalog
                       rdfiltercatalog.cpp
                       FilterCatalog.cpp
                       DEST Chem
                       LINK_LIBRARIES
                       FilterCatalog
Subgraphs SubstructMatch SmilesParse Catalogs FileParsers GraphMol DataStructs
RDGeometryLib RDGeneral RDBoost
)

add_pytest(pyFilterCatalog ${CMAKE_CURRENT_SOURCE_DIR}/rough_test.py)
