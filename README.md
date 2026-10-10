# ADC/DAC Second-Source Evaluation Notes

Practical worksheets for engineers evaluating pin-to-pin candidates on existing converter and RF transceiver boards. Maintained by Leslie at Shenxin Tech.

## ADC worksheets

- [AD9653 / SXA031: four-channel 16-bit ADC and instrument acceptance](docs/ad9653-sxa031-evaluation.md)
- [Blank SXA031 qualification record (CSV)](templates/sxa031-qualification-record.csv)
- [AD9253 / SXA036: four-channel LVDS and instrument acceptance](docs/ad9253-sxa036-evaluation.md)
- [Blank AD9253 qualification record (CSV)](templates/ad9253-sxa036-qualification-record.csv)
- [AD9434 / SXA002: 12-bit 500 MSPS ADC and instrument acceptance](docs/ad9434-sxa002-evaluation.md)
- [Blank SXA002 qualification record (CSV)](templates/sxa002-qualification-record.csv)
- [AD9680 / SXA011: dual-channel 14-bit 1 GSPS ADC and instrument acceptance](docs/ad9680-sxa011-evaluation.md)
- [Blank SXA011 qualification record (CSV)](templates/sxa011-qualification-record.csv)

## DAC worksheets

- [AD9164 / SXD019: JESD204B link and datapath evaluation](docs/ad9164-sxd019-evaluation.md)
- [Blank SXD019 qualification record (CSV)](templates/sxd019-qualification-record.csv)

## RF transceiver worksheets

- [AD9361 / SXS046: 2T2R agile transceiver evaluation, 70 MHz–6 GHz](docs/ad9361-sxs046-evaluation.md)
- [Blank SXS046 qualification record (CSV)](templates/sxs046-qualification-record.csv)
- [AD9363 / SXS055: 2T2R agile transceiver evaluation, 325 MHz–3.8 GHz](docs/ad9363-sxs055-evaluation.md)
- [Blank SXS055 qualification record (CSV)](templates/sxs055-qualification-record.csv)

The worksheets separate package and pin mapping, digital capture, and the finished instrument's own release test. The public files are deliberately blank: they contain no customer measurements, schematics, proprietary pin maps, or claims that a particular board has passed.

SXA031 is Shenxin's 16-bit, four-channel, 125 MSPS pin-to-pin candidate for the matching AD9653 package. SXA036 is Shenxin's 14-bit, four-channel, 125 MSPS pin-to-pin candidate for the matching AD9253 package. AD9253 has 80, 105 and 125 MSPS orderable versions; compare the **complete fitted part number** before applying any equivalence. Pin mapping provides a starting point for an existing PCB evaluation. Electrical, timing, firmware settings and system behavior still require validation.

SXA002 is Shenxin's 12-bit, 500 MSPS pin-to-pin candidate for the matching AD9434 package. SXA011 is Shenxin's dual-channel, 14-bit, 1 GSPS pin-to-pin candidate for the matching AD9680 package. At GSPS rates, clock jitter dominates SNR — compare both devices under identical clock conditions.

SXD019 is Shenxin's 16-bit RF DAC, up to 12 GSPS in 2× NRZ mode (first Nyquist zone), pin-to-pin candidate for AD9164-class BGA169 packages. AD9164 ships in BGA165 and BGA169 — SXD019 is BGA169 only. Verify the fitted package before applying any equivalence.

SXS046 is Shenxin's 2T2R agile transceiver (70 MHz–6 GHz, tunable bandwidth under 200 kHz to 56 MHz, TX EVM −40 dB), pin-to-pin candidate for the matching AD9361 144-BGA 10 × 10 mm package. SXS055 is the industrial-grade 2T2R candidate (325 MHz–3.8 GHz, bandwidth up to 20 MHz, TX EVM −34 dB) for the matching AD9363 package. Verify the fitted package and bandwidth grade before applying any equivalence.

## How to use

1. Copy the CSV into your private project records. Fill one row per acceptance item and board revision.
2. Record the original and candidate under the same clock, input and FPGA conditions.
3. Compare both against the instrument's actual pass/fail criteria. Keep customer data private.
4. If you need the applicable pin comparison or sample-evaluation discussion, contact **Leslie: gjr@shenxinic.com** with the full fitted part code, board revision and test gate.

## Sources and scope

- [Shenxin SXA036 product information](https://shenxinic.com/product/jxa036)
- [Shenxin SXD019 product information](https://shenxinic.com/products)
- [ADI AD9653 product page and data sheet](https://www.analog.com/en/products/ad9653.html)
- [ADI AD9253 product page and data sheet](https://www.analog.com/en/products/ad9253.html)
- [ADI AD9434 product page and data sheet](https://www.analog.com/en/products/ad9434.html)
- [ADI AD9680 product page and data sheet](https://www.analog.com/en/products/ad9680.html)
- [ADI AD9164 product page and data sheet](https://www.analog.com/en/products/ad9164.html)
- [ADI AD9361 product page and data sheet](https://www.analog.com/en/products/ad9361.html)
- [ADI AD9363 product page and data sheet](https://www.analog.com/en/products/ad9363.html)

The templates are evaluation aids, not certifications, test reports, approvals to substitute parts, or commitments about a specific order's price or lead time. Please do not open public issues containing confidential board details, customer identities, patient data or controlled technical information.

*AD9653, AD9253, AD9434, AD9680, AD9164, AD9361 and AD9363 are trademarks of Analog Devices, Inc. SXA031, SXA036, SXA002, SXA011, SXD019, SXS046 and SXS055 are independently designed pin-to-pin alternatives. All trademarks belong to their respective owners.*
