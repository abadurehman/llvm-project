add_llvm_component_library(LLVMFuzzMutate
  FuzzerCLI.cpp
  IRMutator.cpp
  OpDescriptor.cpp
  Operations.cpp
  RandomIRBuilder.cpp

  ADDITIONAL_HEADER_DIRS
  ${LLVM_MAIN_INCLUDE_DIR}/llvm/FuzzMutate

  DEPENDS
  intrinsics_gen
  )
