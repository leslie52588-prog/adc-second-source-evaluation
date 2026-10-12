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
- [AD9213 / SXA050: single-channel 12-bit 10.25 GSPS ADC and instrument acceptance](docs/ad9213-sxa050-evaluation.md)
- [Blank SXA050 qualification record (CSV)](templates/sxa050-qualification-record.csv)
- [AD7960 / SXA004: single-channel 18-bit SAR ADC and instrument acceptance](docs/ad7960-sxa004-evaluation.md)
- [Blank SXA004 qualification record (CSV)](templates/sxa004-qualification-record.csv)
- [AD9467 / SXA008: single-channel 16-bit 250 MSPS ADC and instrument acceptance](docs/ad9467-sxa008-evaluation.md)
- [Blank SXA008 qualification record (CSV)](templates/sxa008-qualification-record.csv)
- [AD9656 / SXA009: four-channel 16-bit 125 MSPS ADC and instrument acceptance](docs/ad9656-sxa009-evaluation.md)
- [Blank SXA009 qualification record (CSV)](templates/sxa009-qualification-record.csv)
- [AD9689 / SXA018: dual-channel 14-bit 2.6 GSPS ADC and instrument acceptance](docs/ad9689-sxa018-evaluation.md)
- [Blank SXA018 qualification record (CSV)](templates/sxa018-qualification-record.csv)
- [AD9245 / SXA021: single-channel 14-bit 50 MSPS ADC and instrument acceptance](docs/ad9245-sxa021-evaluation.md)
- [Blank SXA021 qualification record (CSV)](templates/sxa021-qualification-record.csv)
- [AD9652 / SXA026: dual-channel 16-bit 310 MSPS ADC and instrument acceptance](docs/ad9652-sxa026-evaluation.md)
- [Blank SXA026 qualification record (CSV)](templates/sxa026-qualification-record.csv)
- [AD7606 / SXA029: eight-channel 16-bit simultaneous-sampling ADC and instrument acceptance](docs/ad7606-sxa029-evaluation.md)
- [Blank SXA029 qualification record (CSV)](templates/sxa029-qualification-record.csv)
- [AD9208 / SXA038: dual-channel 14-bit 3 GSPS ADC and instrument acceptance](docs/ad9208-sxa038-evaluation.md)
- [Blank SXA038 qualification record (CSV)](templates/sxa038-qualification-record.csv)

## DAC worksheets

- [AD9164 / SXD019: JESD204B link and datapath evaluation](docs/ad9164-sxd019-evaluation.md)
- [Blank SXD019 qualification record (CSV)](templates/sxd019-qualification-record.csv)
- [AD9154 / SXD020: four-channel 16-bit 2.4 GSPS DAC and instrument acceptance](docs/ad9154-sxd020-evaluation.md)
- [Blank SXD020 qualification record (CSV)](templates/sxd020-qualification-record.csv)
- [AD9122 / SXD033: dual-channel 16-bit 1 GSPS DAC and instrument acceptance](docs/ad9122-sxd033-evaluation.md)
- [Blank SXD033 qualification record (CSV)](templates/sxd033-qualification-record.csv)
- [AD9174 / SXD052: dual-channel 16-bit 11 GSPS RF DAC and instrument acceptance](docs/ad9174-sxd052-evaluation.md)
- [Blank SXD052 qualification record (CSV)](templates/sxd052-qualification-record.csv)

## RF transceiver worksheets

- [AD9361 / SXS046: 2T2R agile transceiver evaluation, 70 MHz–6 GHz](docs/ad9361-sxs046-evaluation.md)
- [Blank SXS046 qualification record (CSV)](templates/sxs046-qualification-record.csv)
- [AD9363 / SXS055: 2T2R agile transceiver evaluation, 325 MHz–3.8 GHz](docs/ad9363-sxs055-evaluation.md)
- [Blank SXS055 qualification record (CSV)](templates/sxs055-qualification-record.csv)

The worksheets separate package and pin mapping, digital capture, and the finished instrument's own release test. The public files are deliberately blank: they contain no customer measurements, schematics, proprietary pin maps, or claims that a particular board has passed.

SXA031 is Shenxin's 16-bit, four-channel, 125 MSPS pin-to-pin candidate for the matching AD9653 package. SXA036 is Shenxin's 14-bit, four-channel, 125 MSPS pin-to-pin candidate for the matching AD9253 package. AD9253 has 80, 105 and 125 MSPS orderable versions; compare the **complete fitted part number** before applying any equivalence. Pin mapping provides a starting point for an existing PCB evaluation. Electrical, timing, firmware settings and system behavior still require validation.

SXA002 is Shenxin's 12-bit, 500 MSPS pin-to-pin candidate for the matching AD9434 package. SXA011 is Shenxin's dual-channel, 14-bit, 1 GSPS pin-to-pin candidate for the matching AD9680 package. At GSPS rates, clock jitter dominates SNR — compare both devices under identical clock conditions.

SXA050 is Shenxin's single-channel, 12-bit, 10.25 GSPS JESD204B pin-to-pin candidate for the matching AD9213 package. SXA004 (18-bit, 5 MSPS SAR) and SXA008 (16-bit, 250 MSPS) are the precision single-channel candidates for AD7960 and AD9467. SXA009 is the four-channel, 16-bit, 125 MSPS candidate for AD9656 — listed grades 80/105/125 MSPS, compare the complete fitted part number. SXA018 is the dual-channel, 14-bit, up to 2.6 GSPS JESD204B candidate for AD9689. SXA021 is the single-channel, 14-bit, up to 50 MSPS parallel-CMOS candidate for AD9245. SXA026 is the dual-channel, 16-bit, up to 310 MSPS LVDS candidate for AD9652. SXA029 is the eight-channel, 16-bit, 200 kSPS simultaneous-sampling candidate for AD7606. SXA038 is the dual-channel, 14-bit, 3 GSPS JESD204B candidate for AD9208. Package and speed-grade details for these newer listings are pending datasheet confirmation — verify the fitted package and grade before applying any equivalence.

SXD019 is Shenxin's 16-bit RF DAC, up to 12 GSPS in 2× NRZ mode (first Nyquist zone), pin-to-pin candidate for AD9164-class BGA169 packages. AD9164 ships in BGA165 and BGA169 — SXD019 is BGA169 only. Verify the fitted package before applying any equivalence.

SXD020 is Shenxin's four-channel, 16-bit, 2.4 GSPS DAC candidate for the matching AD9154 package. SXD033 is the dual-channel, 16-bit, 1 GSPS LVDS DAC candidate for AD9122. SXD052 is the dual-channel, 16-bit, up to 11 GSPS RF DAC candidate for AD9174. Verify the fitted package and JESD204B lane configuration before applying any equivalence.

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
- [ADI AD9213 product page and data sheet](https://www.analog.com/en/products/ad9213.html)
- [ADI AD7960 product page and data sheet](https://www.analog.com/en/products/ad7960.html)
- [ADI AD9467 product page and data sheet](https://www.analog.com/en/products/ad9467.html)
- [ADI AD9656 product page and data sheet](https://www.analog.com/en/products/ad9656.html)
- [ADI AD9689 product page and data sheet](https://www.analog.com/en/products/ad9689.html)
- [ADI AD9245 product page and data sheet](https://www.analog.com/en/products/ad9245.html)
- [ADI AD9652 product page and data sheet](https://www.analog.com/en/products/ad9652.html)
- [ADI AD7606 product page and data sheet](https://www.analog.com/en/products/ad7606.html)
- [ADI AD9208 product page and data sheet](https://www.analog.com/en/products/ad9208.html)
- [ADI AD9154 product page and data sheet](https://www.analog.com/en/products/ad9154.html)
- [ADI AD9122 product page and data sheet](https://www.analog.com/en/products/ad9122.html)
- [ADI AD9174 product page and data sheet](https://www.analog.com/en/products/ad9174.html)

The templates are evaluation aids, not certifications, test reports, approvals to substitute parts, or commitments about a specific order's price or lead time. Please do not open public issues containing confidential board details, customer identities, patient data or controlled technical information.

*AD9653, AD9253, AD9434, AD9680, AD9164, AD9361, AD9363, AD9213, AD7960, AD9467, AD9656, AD9689, AD9245, AD9652, AD7606, AD9208, AD9154, AD9122 and AD9174 are trademarks of Analog Devices, Inc. SXA031, SXA036, SXA002, SXA011, SXA050, SXA004, SXA008, SXA009, SXA018, SXA021, SXA026, SXA029, SXA038, SXD019, SXD020, SXD033, SXD052, SXS046 and SXS055 are independently designed pin-to-pin alternatives. All trademarks belong to their respective owners.*
