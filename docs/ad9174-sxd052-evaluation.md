# AD9174 → SXD052: existing-board evaluation worksheet

**Status:** Public blank method. No measured data or customer board claim.

## Scope

Shenxin lists SXD052 as a pin-to-pin candidate for the matching AD9174 package. The SXD052 listing describes dual-channel, 16-bit, up to 11 GSPS RF DAC operation with a JESD204B interface. Verify the complete ordering suffix, speed grade, package and JESD204B lane configuration; do not infer qualification of every variant from a family name. Package details for SXD052 are pending datasheet confirmation; the AD9174 counterpart ships in 144-ball BGA — confirm the fitted package before applying any equivalence. Speed-grade options are pending datasheet confirmation — verify the fitted grade. At GSPS rates, clock jitter dominates SNR — compare both devices under identical clock conditions.

## 1. Establish the baseline

| Item | Reference AD9174 | Candidate SXD052 | Evidence / reviewer |
|---|---|---|---|
| Full populated ordering code and package | TBD | TBD | TBD |
| PCB revision, fitted options, assembly lot | TBD | TBD | TBD |
| Supply, reference and input full-scale configuration | TBD | TBD | TBD |
| Sample clock source, rate and jitter conditions | TBD | TBD | TBD |
| SPI/register configuration and power-down states | TBD | TBD | TBD |

## 2. Verify the JESD204B link and datapath

Record the link configuration and the DAC datapath modes per the fitted device: interpolation, NCO settings where applicable, lane mapping, FPGA IP core, and the link-establishment procedure. A passing link check confirms the digital path; it does not demonstrate analog or instrument performance.

| Item | Reference | Candidate | Pass criterion |
|---|---|---|---|
| JESD204B subclass, lanes and lane rate | TBD | TBD | TBD |
| Datapath mode: interpolation and NCO configuration | TBD | TBD | TBD |
| Link re-establishment after reset or rate change | TBD | TBD | TBD |

## 3. Repeat the instrument's acceptance test

Use the instrument's own release procedure — for communications or test-equipment builds, the applicable SFDR/ACLR masks, output flatness and temperature range. Record the same clock, output network, gain and software build for each device. Do not publish customer limits or controlled data.

| Test | Reference result | Candidate result | Limit / disposition |
|---|---|---|---|
| SFDR / noise under instrument conditions | TBD | TBD | TBD |
| Output flatness across the band of interest | TBD | TBD | TBD |
| Temperature / repeated build if required | TBD | TBD | TBD |

## Handoff

The result is meaningful only with a board revision, test date, setup, owner and sign-off. A pin match is the beginning of the evaluation. Contact Leslie at **gjr@shenxinic.com** for the matching pin comparison and sample discussion.

Sources: [Shenxin SXD052 product information](https://shenxinic.com/products), [ADI AD9174 product page and data sheet](https://www.analog.com/en/products/ad9174.html).

*AD9174 is a trademark of Analog Devices, Inc. SXD052 is an independently designed pin-to-pin alternative. All trademarks belong to their respective owners.*

