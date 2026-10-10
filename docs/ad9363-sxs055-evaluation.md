# AD9363 → SXS055: existing-board evaluation worksheet

**Status:** Public blank method. No measured data or customer board claim.

## Scope

Shenxin lists SXS055 as a pin-to-pin candidate for the matching AD9363 144-BGA 10 × 10 mm package. SXS055 is a 2T2R agile transceiver: 325 MHz–3.8 GHz, 12-bit ADC/DAC, channel bandwidth up to 20 MHz, TX EVM −34 dB, industrial grade, CMOS/LVDS data interface, TDD/FDD operation, 144-BGA 10 × 10 × 1.42 mm, 0.8 mm ball pitch. Verify the fitted package and bandwidth grade before applying any equivalence. A pin match is the beginning of the evaluation, not a system qualification.

## 1. Establish the baseline

| Item | Reference AD9363 | Candidate SXS055 | Evidence / reviewer |
|---|---|---|---|
| Full populated ordering code and package | TBD | TBD | TBD |
| PCB revision, fitted options, assembly lot | TBD | TBD | TBD |
| Supply rails and reference clock source/rate | TBD | TBD | TBD |
| SPI/register configuration, TDD/FDD mode | TBD | TBD | TBD |
| Channel bandwidth and filter profile | TBD | TBD | TBD |

## 2. Verify the digital data interface

Record the data-port mode (CMOS/LVDS), sample clock, I/Q framing, FPGA bitstream and any loopback or test-tone procedure per the fitted configuration. A clean loopback checks the digital path; it does not demonstrate RF performance.

| Item | Reference | Candidate | Pass criterion |
|---|---|---|---|
| Data-port mode and I/Q capture | TBD | TBD | TBD |
| Sample clock and framing alignment | TBD | TBD | TBD |
| Loopback / test-tone integrity | TBD | TBD | TBD |

## 3. Run RF acceptance on your board

Use your own RF acceptance procedure — EVM, phase noise, spurious and image rejection under your band, bandwidth and temperature conditions. Record the same RF matching, clocking, supply and software state for each device. A pin match starts the evaluation; it does not finish it. Do not publish customer limits or controlled data.

| Test | Reference result | Candidate result | Limit / disposition |
|---|---|---|---|
| TX EVM at operating bandwidth | TBD | TBD | TBD |
| Phase noise and spurious | TBD | TBD | TBD |
| Image rejection / I/Q balance | TBD | TBD | TBD |
| Temperature / repeated build if required | TBD | TBD | TBD |

## Handoff

The result is meaningful only with a board revision, test date, setup, owner and sign-off. Contact Leslie at **gjr@shenxinic.com** with the full fitted part code and board revision for the applicable pin comparison and sample discussion.

Sources: [Shenxin SXS055 product information](https://shenxinic.com/products), [ADI AD9363 product page and data sheet](https://www.analog.com/en/products/ad9363.html).

*AD9363 is a trademark of Analog Devices, Inc. SXS055 is an independently designed pin-to-pin alternative. All trademarks belong to their respective owners.*
