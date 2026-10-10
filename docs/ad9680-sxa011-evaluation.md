# AD9680 → SXA011: existing-board evaluation worksheet

**Status:** Public blank method. No measured data or customer board claim.

## Scope

Shenxin lists SXA011 as a pin-to-pin candidate for the matching AD9680 package. The SXA011 listing describes dual-channel, 14-bit, 1 GSPS operation. Verify the complete ordering suffix, speed grade, package and JESD204B configuration; do not infer qualification of every variant from a family name.

## 1. Establish the baseline

| Item | Reference AD9680 | Candidate SXA011 | Evidence / reviewer |
|---|---|---|---|
| Full populated ordering code and package | TBD | TBD | TBD |
| PCB revision, fitted options, assembly lot | TBD | TBD | TBD |
| Supply, reference and input full-scale configuration | TBD | TBD | TBD |
| Sample clock source, rate and jitter conditions | TBD | TBD | TBD |
| SPI/register configuration and power-down states | TBD | TBD | TBD |

## 2. Verify the JESD204B link

Record lane count, per-lane rate, subclass, LMFC alignment, SYNC behavior and link test patterns per the fitted configuration. A locked link checks the digital path; it does not demonstrate analog or system performance. At 1 GSPS, clock jitter dominates SNR — record the clock source phase noise for both devices under identical conditions.

| Item | Reference | Candidate | Pass criterion |
|---|---|---|---|
| Lane rate, subclass and LMFC alignment | TBD | TBD | TBD |
| Link establishment and re-sync behavior | TBD | TBD | TBD |
| Test-pattern integrity across all lanes | TBD | TBD | TBD |

## 3. Repeat the instrument's acceptance test

Use the instrument's own release procedure — for 5G, wideband-receiver or test-equipment builds, the applicable SFDR/SNR masks, channel flatness and temperature range. Record the same clock, input network, gain and software build for each device. Do not publish customer limits or controlled data.

| Test | Reference result | Candidate result | Limit / disposition |
|---|---|---|---|
| SFDR / SNR under instrument conditions | TBD | TBD | TBD |
| Wideband flatness and spurious plan | TBD | TBD | TBD |
| Temperature / repeated build if required | TBD | TBD | TBD |

## Handoff

The result is meaningful only with a board revision, test date, setup, owner and sign-off. A pin match is the beginning of the evaluation. Contact Leslie at **gjr@shenxinic.com** for the matching pin comparison and sample discussion.

Sources: [Shenxin SXA011 product information](https://shenxinic.com/products), [ADI AD9680 product page and data sheet](https://www.analog.com/en/products/ad9680.html).

*AD9680 is a trademark of Analog Devices, Inc. SXA011 is an independently designed pin-to-pin alternative. All trademarks belong to their respective owners.*
