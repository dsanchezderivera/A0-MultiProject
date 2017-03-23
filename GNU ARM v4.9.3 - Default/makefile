################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include src/subdir.mk
-include kit_lcd/BRD4300C/subdir.mk
-include kit/BRD4300C/subdir.mk
-include glib/BRD4300C/subdir.mk
-include emlib/subdir.mk
-include device/EFR32_B_1_1_B/gcc/subdir.mk
-include bgapi/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: A0-MultiProject.axf

# Tool invocations
A0-MultiProject.axf: $(OBJS) $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Invoking: GNU ARM C Linker'
	arm-none-eabi-gcc -g -gdwarf-2 -mcpu=cortex-m4 -mthumb -T "C:\Users\Diego\SimplicityStudio\v4_workspace\A0-MultiProject\linker\GCC\efr32bg1b232f256gm48.ld" -Xlinker -no-enum-size-warning -Xlinker -no-wchar-size-warning -Xlinker --gc-sections -Xlinker -Map="A0-MultiProject.map" -mfpu=fpv4-sp-d16 -mfloat-abi=softfp -o A0-MultiProject.axf "./advertisement.o" "./app.o" "./app_hw.o" "./app_ui.o" "./application_properties.o" "./beacon.o" "./ble-callback-stubs.o" "./ble-callbacks.o" "./gatt_db.o" "./graphics.o" "./htm.o" "./ia.o" "./main.o" "./bgapi/dmadrv.o" "./bgapi/em_adc.o" "./bgapi/em_ldma.o" "./bgapi/em_leuart.o" "./device/EFR32_B_1_1_B/gcc/startup_efr32bg1b.o" "./emlib/em_cmu.o" "./emlib/em_cryotimer.o" "./emlib/em_emu.o" "./emlib/em_gpio.o" "./emlib/em_i2c.o" "./emlib/em_msc.o" "./emlib/em_rtcc.o" "./emlib/em_system.o" "./emlib/em_usart.o" "./glib/BRD4300C/bmp.o" "./glib/BRD4300C/dmd_display.o" "./glib/BRD4300C/glib.o" "./glib/BRD4300C/glib_bitmap.o" "./glib/BRD4300C/glib_circle.o" "./glib/BRD4300C/glib_font_narrow_6x8.o" "./glib/BRD4300C/glib_font_normal_8x8.o" "./glib/BRD4300C/glib_font_number_16x20.o" "./glib/BRD4300C/glib_line.o" "./glib/BRD4300C/glib_polygon.o" "./glib/BRD4300C/glib_rectangle.o" "./glib/BRD4300C/glib_string.o" "./kit/BRD4300C/bsp_bcc.o" "./kit/BRD4300C/bsp_stk.o" "./kit/BRD4300C/bsp_stk_leds.o" "./kit/BRD4300C/i2cspm.o" "./kit/BRD4300C/si7013.o" "./kit/BRD4300C/tempsens.o" "./kit/BRD4300C/udelay.o" "./kit_lcd/BRD4300C/display.o" "./kit_lcd/BRD4300C/displayls013b7dh03.o" "./kit_lcd/BRD4300C/displaypalemlib.o" "./src/InitDevice.o" "C:/SiliconLabs/SimplicityStudio/v4/developer/sdks/gecko_sdk_suite/v1.0//protocol/bluetooth_2.3/lib/EFR32BG1B/EABI/binbootloader.o" "C:/SiliconLabs/SimplicityStudio/v4/developer/sdks/gecko_sdk_suite/v1.0//protocol/bluetooth_2.3/lib/EFR32BG1B/GCC/bgapi.a" "C:/SiliconLabs/SimplicityStudio/v4/developer/sdks/gecko_sdk_suite/v1.0//protocol/bluetooth_2.3/lib/EFR32BG1B/EABI/stack.a" "C:/SiliconLabs/SimplicityStudio/v4/developer/sdks/gecko_sdk_suite/v1.0//protocol/bluetooth_2.3/lib/EFR32BG1B/EABI/binstack.o" -lm -Wl,--start-group -lgcc -lc -lnosys -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

	@echo 'Building hex file: A0-MultiProject.hex'
	arm-none-eabi-objcopy -O ihex "A0-MultiProject.axf" "A0-MultiProject.hex"
	@echo ' '

	@echo 'Building bin file: A0-MultiProject.bin'
	arm-none-eabi-objcopy -O binary "A0-MultiProject.axf" "A0-MultiProject.bin"
	@echo ' '

	@echo 'Building s37 file: A0-MultiProject.s37'
	arm-none-eabi-objcopy -O srec "A0-MultiProject.axf" "A0-MultiProject.s37"
	@echo ' '

	@echo 'Running size tool'
	arm-none-eabi-size "A0-MultiProject.axf"
	@echo ' '

# Other Targets
clean:
	-$(RM) $(EXECUTABLES)$(OBJS)$(C_DEPS) A0-MultiProject.axf
	-@echo ' '

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets
