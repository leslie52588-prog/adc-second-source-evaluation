# ADC/DAC Second-Source Evaluation Notes

Practical worksheets for engineers evaluating pin-to-pin candidates on existing converter boards. Maintained by Leslie at Shenxin Tech.

## Start here

- [AD9253 / SXA036: four-channel LVDS and instrument acceptance](docs/ad9253-sxa036-evaluation.md)
- [Blank AD9253 qualification record (CSV)](templates/ad9253-sxa036-qualification-record.csv)
- [AD9164 / SXD019: JESD204B link and datapath evaluation](docs/ad9164-sxd019-evaluation.md)
- [Blank SXD019 qualification record (CSV)](templates/sxd019-qualification-record.csv)

The worksheets separate package and pin mapping, digital capture, and the finished instrument's own release test. The public files are deliberately blank: they contain no customer measurements, schematics, proprietary pin maps, or claims that a particular board has passed.

SXA036 is Shenxin's 14-bit, four-channel, 125 MSPS pin-to-pin candidate for the matching AD9253 package. AD9253 has 80, 105 and 125 MSPS orderable versions; compare the **complete fitted part number** before applying any equivalence. Pin mapping provides a starting point for an existing PCB evaluation. Electrical, timing, firmware settings and system behavior still require validation.

SXD019 is Shenxin's 16-bit RF DAC, up to 12 GSPS in 2× NRZ mode (first Nyquist zone), pin-to-pin candidate for AD9164-class BGA169 packages. AD9164 ships in BGA165 and BGA169 — SXD019 is BGA169 only. Verify the fitted package before applying any equivalence.

## How to use

1. Copy the CSV into your private project records. Fill one row per acceptance item and board revision.
2. Record the original and candidate under the same clock, input and FPGA conditions.
3. Compare both against the instrument's actual pass/fail criteria. Keep customer data private.
4. If you need the applicable pin comparison or sample-evaluation discussion, contact **Leslie: gjr@shenxinic.com** with the full fitted part code, board revision and test gate.

## Sources and scope

- [Shenxin SXA036 product information](https://shenxinic.com/product/jxa036)
- [Shenxin SXD019 product information](https://shenxinic.com/product/sxd019)
- [ADI AD9253 product page and data sheet](https://www.analog.com/en/products/ad9253.html)
- [ADI AD9164 product page and data sheet](https://www.analog.com/en/products/ad9164.html)

The templates are evaluation aids, not certifications, test reports, approvals to substitute parts, or commitments about a specific order's price or lead time. Please do not open public issues containing confidential board details, customer identities, patient data or controlled technical information.

*AD9253 and AD9164 are trademarks of Analog Devices, Inc. SXA036 and SXD019 are independently designed pin-to-pin alternatives. All trademarks belong to their respective owners.*
