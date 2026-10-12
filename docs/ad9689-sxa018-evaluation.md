# AD9689 → SXA018: existing-board evaluation worksheet

**Status:** Public blank method. No measured data or customer board claim.

## Scope

Shenxin lists SXA018 as a pin-to-pin candidate for the matching AD9689 package. The SXA018 listing describes dual-channel, 14-bit, up to 2.6 GSPS operation with a JESD204B interface. Verify the complete ordering suffix, speed grade, package and JESD204B lane configuration; do not infer qualification of every variant from a family name. Package details for SXA018 are pending datasheet confirmation; the AD9689 counterpart ships in BGA package — confirm the fitted package before applying any equivalence. Speed-grade options are pending datasheet confirmation — verify the fitted grade. At GSPS rates, clock jitter dominates SNR — compare both devices under identical clock conditions.

## 1. Establish the baseline

| Item | Reference AD9689 | Candidate SXA018 | Evidence / reviewer |
|---|---|---|---|
| Full populated ordering code and package | TBD | TBD | TBD |
| PCB revision, fitted options, assembly lot | TBD | TBD | TBD |
| Supply, reference and input full-scale configuration | TBD | TBD | TBD |
| Sample clock source, rate and jitter conditions | TBD | TBD | TBD |
| SPI/register configuration and power-down states | TBD | TBD | TBD |

## 2. Verify the JESD204B link

Record the link configuration per the fitted device: lane rate, subclass and SYSREF handling, FPGA IP core, and the link-establishment procedure. A passing link check confirms the digital path; it does not demonstrate analog or instrument performance.

| Item | Reference | Candidate | Pass criterion |
|---|---|---|---|
| JESD204B subclass, lanes and lane rate | TBD | TBD | TBD |
| SYSREF / sync and deterministic latency | TBD | TBD | TBD |
| Link re-establishment after reset or rate change | TBD | TBD | TBD |

## 3. Repeat the instrument's acceptance test

Use the instrument's own release procedure — for communications, base-station or test-equipment builds, the applicable SFDR/SNR masks, channel flatness and temperature range. Record the same clock, input network, gain and software build for each device. Do not publish customer limits or controlled data.

| Test | Reference result | Candidate result | Limit / disposition |
|---|---|---|---|
| SFDR / SNR under instrument conditions | TBD | TBD | TBD |
| Channel flatness across the band of interest | TBD | TBD | TBD |
| Temperature / repeated build if required | TBD | TBD | TBD |

## Handoff

The result is meaningful only with a board revision, test date, setup, owner and sign-off. A pin match is the beginning of the evaluation. Contact Leslie at **gjr@shenxinic.com** for the matching pin comparison and sample discussion.

Sources: [Shenxin SXA018 product information](https://shenxinic.com/products), [ADI AD9689 product page and data sheet](https://www.analog.com/en/products/ad9689.html).

*AD9689 is a trademark of Analog Devices, Inc. SXA018 is an independently designed pin-to-pin alternative. All trademarks belong to their respective owners.*

