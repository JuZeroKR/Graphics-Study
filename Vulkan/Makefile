ASSEMBLY:= Engine
BUILD_DIR:= bin

COMPILER_FLAGS:= -std=c2x
INCLUDE_FLAGS:= -IEngine/src -I$(VULKAN_SDK)/include -I$(VULKAN_SDK)/lib
LINKER_FLAGS:= -lvulkan
SRC_FILES:= $(shell find $(ASSEMBLY) -type f \( -name "*.c" -o -name "*.m" \))

.PHONY: build
build:
	@clang $(COMPILER_FLAGS) $(SRC_FILES) -o $(BUILD_DIR)/app $(INCLUDE_FLAGS) $(LINKER_FLAGS)