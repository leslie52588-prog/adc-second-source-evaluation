# AD9122 → SXD033: existing-board evaluation worksheet

**Status:** Public blank method. No measured data or customer board claim.

## Scope

Shenxin lists SXD033 as a pin-to-pin candidate for the matching AD9122 package. The SXD033 listing describes dual-channel, 16-bit, 1 GSPS DAC operation with an LVDS data interface. Verify the complete ordering suffix, speed grade, package and LVDS data-interface configuration; do not infer qualification of every variant from a family name. Package details for SXD033 are pending datasheet confirmation; the AD9122 counterpart ships in 72-lead LFCSP (10 × 10 mm) — confirm the fitted package before applying any equivalence. Listed speed grade (1 GSPS) is per internal cross-reference — verify the fitted grade.

## 1. Establish the baseline

| Item | Reference AD9122 | Candidate SXD033 | Evidence / reviewer |
|---|---|---|---|
| Full populated ordering code and package | TBD | TBD | TBD |
| PCB revision, fitted options, assembly lot | TBD | TBD | TBD |
| Supply, reference and input full-scale configuration | TBD | TBD | TBD |
| Sample clock source, rate and jitter conditions | TBD | TBD | TBD |
| SPI/register configuration and power-down states | TBD | TBD | TBD |

## 2. Verify the LVDS datapath

Record the LVDS data interface mode per the fitted configuration, clock/data timing relationship, FPGA bitstream, and any test-pattern procedure. A passing test pattern checks the data path; it does not demonstrate analog or instrument performance.

| Item | Reference | Candidate | Pass criterion |
|---|---|---|---|
| Data interface mode and capture timing | TBD | TBD | TBD |
| Data integrity and alignment | TBD | TBD | TBD |
| Restart and operating-mode transitions | TBD | TBD | TBD |

## 3. Repeat the instrument's acceptance test

Use the instrument's own release procedure — for communications or test-equipment builds, the applicable SFDR/ACLR masks, output flatness and temperature range. Record the same clock, output network, gain and software build for each device. Do not publish customer limits or controlled data.

| Test | Reference result | Candidate result | Limit / disposition |
|---|---|---|---|
| SFDR / noise under instrument conditions | TBD | TBD | TBD |
| Output flatness across the band of interest | TBD | TBD | TBD |
| Temperature / repeated build if required | TBD | TBD | TBD |

## Handoff

The result is meaningful only with a board revision, test date, setup, owner and sign-off. A pin match is the beginning of the evaluation. Contact Leslie at **gjr@shenxinic.com** for the matching pin comparison and sample discussion.

Sources: [Shenxin SXD033 product information](https://shenxinic.com/products), [ADI AD9122 product page and data sheet](https://www.analog.com/en/products/ad9122.html).

*AD9122 is a trademark of Analog Devices, Inc. SXD033 is an independently designed pin-to-pin alternative. All trademarks belong to their respective owners.*

