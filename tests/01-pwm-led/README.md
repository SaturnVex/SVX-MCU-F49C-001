# LED & Gate-Drive PWM Test

**Board:** `SVX-MCU-F49C-001` · **MCU:** TMS320F280049C (F280049CPZS)

Toggle LED1 / LED2 at 500 Hz and blink LED_Status at 1 Hz, and generate 45 kHz center-aligned PWM with 500 ns dead time on all twelve INH / INL gate-drive outputs of motor A and motor B. The gate drivers stay disabled, so only the logic-level gate signals are checked.

## Files

- [Test setup, connections, import/build and acceptance guide (PDF)](SaturnVex_F280049C_PWM_LED_Test_Guide_EN.pdf)
- [Code Composer Studio source project (ZIP)](F280049C_PWM_LED_Test_SaturnVex.zip?raw=true)

## Run this test

1. Read the PDF guide and confirm the hardware connections and prerequisites.
2. Download and extract `F280049C_PWM_LED_Test_SaturnVex.zip`, preserving the project files.
3. In Code Composer Studio select File → Import → CCS Projects, choose the extracted `F280049C_PWM_LED_Test` folder, set the `CPU1_FLASH` configuration, build and program through the JTAG debug probe, following the guide.
4. Verify the results using the PDF acceptance criteria.

SaturnVex files are provided under the BSD-3-Clause license (`LICENSE.txt`). TI C2000Ware files keep their own copyright notices (`NOTICE.txt`); preserve them when redistributing.

[← All tests](../README.md) · [← Product home](../../README.md)
