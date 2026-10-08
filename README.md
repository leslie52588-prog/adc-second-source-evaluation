# ADC Second-Source Evaluation Notes

Practical worksheets for engineers evaluating a pin-to-pin candidate on an existing converter board. Maintained by Leslie at Shenxin Tech.

## Start here

- [AD9253 / JXA036: four-channel LVDS and instrument acceptance](docs/ad9253-jxa036-evaluation.md)
- [Blank qualification record (CSV)](templates/ad9253-qualification-record.csv)

The worksheet separates package and pin mapping, digital capture, and the finished instrument's own release test. The public file is deliberately blank: it contains no customer measurements, schematic, proprietary pin map, or claim that a particular board has passed.

JXA036 is Shenxin's 14-bit, four-channel, 125 MSPS pin-to-pin candidate for the matching AD9253 package. AD9253 has 80, 105 and 125 MSPS orderable versions; compare the **complete fitted part number** before applying any equivalence. Pin mapping provides a starting point for an existing PCB evaluation. Electrical, timing, firmware settings and system behavior still require validation.

## How to use

1. Copy the CSV into your private project records. Fill one row per acceptance item and board revision.
2. Record the original and candidate under the same clock, input and FPGA conditions.
3. Compare both against the instrument's actual pass/fail criteria. Keep customer data private.
4. If you need the applicable pin comparison or sample-evaluation discussion, contact **Leslie: gjr@shenxinic.com** with the full fitted part code, board revision and test gate.

## Sources and scope

- [Shenxin JXA036 product information](https://shenxinic.com/product/jxa036)
- [ADI AD9253 product page and data sheet](https://www.analog.com/en/products/ad9253.html)

The template is an evaluation aid, not a certification, test report, approval to substitute a part, or a commitment about a specific order's price or lead time. Please do not open public issues containing confidential board details, customer identities, patient data or controlled technical information.
