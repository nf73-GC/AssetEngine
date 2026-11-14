# CMakeList.txt : projet CMake pour AssetEngine, incluez la source et définissez
# la logique spécifique au projet ici.
#

# Ajoutez une source à l'exécutable de ce projet.
add_executable (AssetEngine "AssetEngine.cpp" "AssetEngine.h")

target_link_libraries(AssetEngine PRIVATE htn)

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET AssetEngine PROPERTY CXX_STANDARD 20)
endif()

# TODO: Ajoutez des tests et installez des cibles si nécessaire.
