# AD9652 → SXA026: existing-board evaluation worksheet

**Status:** Public blank method. No measured data or customer board claim.

## Scope

Shenxin lists SXA026 as a pin-to-pin candidate for the matching AD9652 package. The SXA026 listing describes dual-channel, 16-bit, up to 310 MSPS operation with an LVDS serial interface. Verify the complete ordering suffix, speed grade, package and serial-interface configuration; do not infer qualification of every variant from a family name. Package details for SXA026 are pending datasheet confirmation; the AD9652 counterpart ships in 64-lead QFN (9 × 9 mm) — confirm the fitted package before applying any equivalence. Listed speed grades (260/310 MSPS grades) are per internal cross-reference — verify the fitted grade.

## 1. Establish the baseline

| Item | Reference AD9652 | Candidate SXA026 | Evidence / reviewer |
|---|---|---|---|
| Full populated ordering code and package | TBD | TBD | TBD |
| PCB revision, fitted options, assembly lot | TBD | TBD | TBD |
| Supply, reference and input full-scale configuration | TBD | TBD | TBD |
| Sample clock source, rate and jitter conditions | TBD | TBD | TBD |
| SPI/register configuration and power-down states | TBD | TBD | TBD |

## 2. Verify digital capture

Record the serial output mode per the fitted configuration, lane/clock relationship, FPGA bitstream, capture timing and any test-pattern procedure. A passing test pattern checks the data path; it does not demonstrate analog or instrument performance.

| Item | Reference | Candidate | Pass criterion |
|---|---|---|---|
| Serial interface mode and lane capture | TBD | TBD | TBD |
| Data integrity and alignment | TBD | TBD | TBD |
| Restart and operating-mode transitions | TBD | TBD | TBD |

## 3. Repeat the instrument's acceptance test

Use the instrument's own release procedure — for communications, base-station or test-equipment builds, the applicable SFDR/SNR masks, channel flatness and temperature range. Record the same clock, input network, gain and software build for each device. Do not publish customer limits or controlled data.

| Test | Reference result | Candidate result | Limit / disposition |
|---|---|---|---|
| SFDR / SNR under instrument conditions | TBD | TBD | TBD |
| Channel flatness across the band of interest | TBD | TBD | TBD |
| Temperature / repeated build if required | TBD | TBD | TBD |

## Handoff

The result is meaningful only with a board revision, test date, setup, owner and sign-off. A pin match is the beginning of the evaluation. Contact Leslie at **gjr@shenxinic.com** for the matching pin comparison and sample discussion.

Sources: [Shenxin SXA026 product information](https://shenxinic.com/products), [ADI AD9652 product page and data sheet](https://www.analog.com/en/products/ad9652.html).

*AD9652 is a trademark of Analog Devices, Inc. SXA026 is an independently designed pin-to-pin alternative. All trademarks belong to their respective owners.*

