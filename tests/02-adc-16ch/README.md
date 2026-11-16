# 16-Channel ADC Measurement Test

**Board:** `SVX-MCU-F49C-001` · **MCU:** TMS320F280049C (F280049CPZS)

Sample all 16 analog inputs (phase currents, phase voltages and DC bus of both motors, plus two NTC inputs) at 1 kHz with the internal 3.3 V reference and read voltages, raw codes and noise statistics live in the CCS Expressions view.

## Files

- [Test setup, connections, import/build and acceptance guide (PDF)](SaturnVex_F280049C_ADC_Test_Guide_EN.pdf)
- [Code Composer Studio source project (ZIP)](F280049C_ADC_Test_SaturnVex.zip?raw=true)

## Run this test

1. Read the PDF guide and confirm the hardware connections and prerequisites.
2. Download and extract `F280049C_ADC_Test_SaturnVex.zip`, preserving the project files.
3. In Code Composer Studio select File → Import → CCS Projects, choose the extracted `F280049C_ADC_Test` folder, set the `CPU1_FLASH` configuration, build and program through the JTAG debug probe, following the guide.
4. Verify the results using the PDF acceptance criteria.

SaturnVex files are provided under the BSD-3-Clause license (`LICENSE.txt`). TI C2000Ware files keep their own copyright notices (`NOTICE.txt`); preserve them when redistributing.

[← All tests](../README.md) · [← Product home](../../README.md)
