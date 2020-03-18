set(LLVM_LINK_COMPONENTS
  Support
  )

add_toy_chapter(toyc-str
  toyc.cpp
  parser/AST.cpp
  )
include_directories(include/)
target_link_libraries(toyc-str
  PRIVATE
    MLIRSupport)
