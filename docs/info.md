<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

This project implements an 8-bit combinational adder.

The 8-bit input `ui_in` and the 8-bit input `uio_in` are added together. The resulting value is provided at the 8-bit output `uo_out`.

The basic operation is:

`uo_out = ui_in + uio_in`


## How to test

Apply different 8-bit values to `ui_in` and `uio_in` and verify that `uo_out` is equal to their sum.

For example:

| `ui_in` | `uio_in` | Expected `uo_out` |
|---:|---:|---:|
| 5 | 3 | 8 |
| 10 | 20 | 30 |
| 100 | 50 | 150 |
| 255 | 1 | 0* |

\* Since `uo_out` is only 8 bits wide, the result wraps around modulo 256.
## External hardware

List external hardware used in your project (e.g. PMOD, LED display, etc), if any
