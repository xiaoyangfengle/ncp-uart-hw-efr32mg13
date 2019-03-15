################################################################################
# Automatically-generated file. Do not edit!
################################################################################

export WINEDEBUG=-all

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include sim-eeprom2/EFR32_1/subdir.mk
-include serial/EFR32/subdir.mk
-include serial/subdir.mk
-include secure-ezsp-stub/subdir.mk
-include ncp-uart/subdir.mk
-include led/EFR32/subdir.mk
-include hal-library/EFR32/subdir.mk
-include external-generated-files/subdir.mk
-include emlib/subdir.mk
-include emdrv/subdir.mk
-include ember-minimal-printf/subdir.mk
-include diagnostic/EFR32/subdir.mk
-include debug-channel/EFR32/subdir.mk
-include debug-basic-library/EFR32/subdir.mk
-include coexistence/EFR32/subdir.mk
-include buzzer-stub/subdir.mk
-include button-stub/subdir.mk
-include build/obj/subdir.mk
-include antenna-stub/subdir.mk
-include adc/EFR32/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(ASM_UPPER_DEPS)),)
-include $(ASM_UPPER_DEPS)
endif
ifneq ($(strip $(MSA_UPPER_DEPS)),)
-include $(MSA_UPPER_DEPS)
endif
ifneq ($(strip $(ASM_DEPS)),)
-include $(ASM_DEPS)
endif
ifneq ($(strip $(S79_DEPS)),)
-include $(S79_DEPS)
endif
ifneq ($(strip $(S_DEPS)),)
-include $(S_DEPS)
endif
ifneq ($(strip $(S_UPPER_DEPS)),)
-include $(S_UPPER_DEPS)
endif
ifneq ($(strip $(MSA_DEPS)),)
-include $(MSA_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
ifneq ($(strip $(S79_UPPER_DEPS)),)
-include $(S79_UPPER_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: pre-build main-build

# Main-build Target
main-build: ncp-uart-hw-efr32mg13.out

# Tool invocations
ncp-uart-hw-efr32mg13.out: $(OBJS) $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Invoking: IAR Linker for ARM'
	@echo 'Adding linker inputs to ilinkCommandLine_ncp-uart-hw-efr32mg13.out.xcl'
	echo. $(foreach file,$(OBJS), $(file)) >> ilinkCommandLine_ncp-uart-hw-efr32mg13.out.xcl
	echo. $(foreach file,$(USER_OBJS), $(file)) >> ilinkCommandLine_ncp-uart-hw-efr32mg13.out.xcl
	@echo 'Invoking linker reading args from file: ilinkCommandLine_ncp-uart-hw-efr32mg13.out.xcl'
	ilinkarm -f "C:\Users\sven.yang\SimplicityStudio\v4_workspace\ncp-uart-hw-efr32mg13\IAR ARM - Default - EFR32MG13P732F512GM48\ilinkCommandLine_ncp-uart-hw-efr32mg13.out.xcl" 
	ielftool --srec --verbose "ncp-uart-hw-efr32mg13.out" "ncp-uart-hw-efr32mg13.s37"  
	ielftool --ihex --verbose "ncp-uart-hw-efr32mg13.out" "ncp-uart-hw-efr32mg13.hex"  
	ielftool --bin --verbose "ncp-uart-hw-efr32mg13.out" "ncp-uart-hw-efr32mg13.bin"
	@echo 'Finished building target: $@'
	@echo ' '
	$(MAKE) --no-print-directory post-build

# Other Targets
clean:
	-$(RM) $(ASM_UPPER_DEPS)$(MSA_UPPER_DEPS)$(EXECUTABLES)$(OBJS)$(ASM_DEPS)$(S79_DEPS)$(S_DEPS)$(S_UPPER_DEPS)$(MSA_DEPS)$(C_DEPS)$(S79_UPPER_DEPS) ncp-uart-hw-efr32mg13.out
	-@echo ' '

pre-build:
	-cmd //c 'C:\Users\SVEN~1.YAN\SIMPLI~1\V4_WOR~1\NCP-UA~1/ncp-uart-hw-efr32mg13-prebuild.bat' 'ncp-uart-hw-efr32mg13' 'C:/Users/sven.yang/SimplicityStudio/v4_workspace/ncp-uart-hw-efr32mg13' 'D:/Program Files (x86)/IAR Systems/Embedded Workbench 8.1/arm' 'C:\SiliconLabs\SimplicityStudio\v4'
	-@echo ' '

post-build:
	-cmd //c 'C:\Users\SVEN~1.YAN\SIMPLI~1\V4_WOR~1\NCP-UA~1/ncp-uart-hw-efr32mg13-postbuild.bat' 'ncp-uart-hw-efr32mg13' 'C:/Users/sven.yang/SimplicityStudio/v4_workspace/ncp-uart-hw-efr32mg13' 'D:/Program Files (x86)/IAR Systems/Embedded Workbench 8.1/arm' 'C:\SiliconLabs\SimplicityStudio\v4'
	-@echo ' '

.PHONY: all clean dependents
.SECONDARY: main-build pre-build post-build

-include ../makefile.targets
