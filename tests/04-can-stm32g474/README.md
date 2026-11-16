# CAN 2.0 Communication Test with STM32G474

**Board:** `SVX-MCU-F49C-001` · **MCU:** TMS320F280049C (F280049CPZS)

Two-way classic CAN 2.0A communication at 500 kbps between this board and the SaturnVex STM32G474 board (SVX-MCU-STM32G474-001). Each board sends one 8-byte frame per second and checks every received frame for identifier, data pattern and lost frames; results are printed on both debug UARTs.

## Files

- [Test setup, connections, import/build and acceptance guide (PDF)](SaturnVex_F280049C_CAN_Test_Guide_EN.pdf)
- [Source projects (ZIP): `F280049C_CAN_Test` for Code Composer Studio and the partner project `STM32G474_CAN_F280049C_Test` for STM32CubeIDE](F280049C_CAN_Test_SaturnVex.zip?raw=true)

## Run this test

1. Read the PDF guide and confirm the hardware connections and prerequisites.
2. Download and extract `F280049C_CAN_Test_SaturnVex.zip`, preserving the project files.
3. In Code Composer Studio select File → Import → CCS Projects, choose the extracted `F280049C_CAN_Test` folder, set the `CPU1_FLASH` configuration, build and program through the JTAG debug probe, following the guide.
4. Import the `STM32G474_CAN_F280049C_Test` folder from the same ZIP into STM32CubeIDE, build and flash it with ST-LINK, then wire CAN_H, CAN_L and GND between the boards as described in the guide.
5. Verify the results using the PDF acceptance criteria.

SaturnVex files are provided under the BSD-3-Clause license (`LICENSE.txt`). TI C2000Ware files keep their own copyright notices (`NOTICE.txt`); preserve them when redistributing. The STM32G474 partner project contains STMicroelectronics HAL / CubeMX-generated code and Arm CMSIS, which keep their own licenses.

[← All tests](../README.md) · [← Product home](../../README.md)
