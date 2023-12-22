set(LLVM_LINK_COMPONENTS
  Support
  )

llvm_add_library(LLVMTableGenGlobalISel STATIC DISABLE_LLVM_LINK_LLVM_DYLIB
                 CodeExpander.cpp
                 GIMatchDag.cpp
                 GIMatchDagEdge.cpp
                 GIMatchDagInstr.cpp
                 GIMatchDagOperands.cpp
                 GIMatchDagPredicate.cpp
                 GIMatchDagPredicateDependencyEdge.cpp
                 GIMatchTree.cpp
                )

set(LLVM_LINK_COMPONENTS
                Support_NOE
                )
llvm_add_library(LLVMTableGenGlobalISel_NOE STATIC DISABLE_LLVM_LINK_LLVM_DYLIB
                 CodeExpander.cpp
                 GIMatchDag.cpp
                 GIMatchDagEdge.cpp
                 GIMatchDagInstr.cpp
                 GIMatchDagOperands.cpp
                 GIMatchDagPredicate.cpp
                 GIMatchDagPredicateDependencyEdge.cpp
                 GIMatchTree.cpp
                )