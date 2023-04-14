This sample shows how to use nRF7002 with a non-Nordic host on vanilla zephyr.

When target is 52840DK, run

	west build -b nrf52840dk_nrf52840 ./ -p -DSHIELD="nrf7002_ek"

When target is nucleo_f412zg, run

	west build -b nucleo_f412zg ./ -p -DSHIELD="nrf7002_ek" -DCONF_FILE="prj-stm32.conf" -DDTC_OVERLAY_FILE="dts-stm32.overlay"