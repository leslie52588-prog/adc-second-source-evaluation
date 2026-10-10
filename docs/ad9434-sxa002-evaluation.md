# AD9434 → SXA002: existing-board evaluation worksheet

**Status:** Public blank method. No measured data or customer board claim.

## Scope

Shenxin lists SXA002 as a pin-to-pin candidate for the matching AD9434 package. The SXA002 listing describes 12-bit, 500 MSPS operation. Verify the complete ordering suffix, speed grade, package and serial-interface configuration; do not infer qualification of every variant from a family name.

## 1. Establish the baseline

| Item | Reference AD9434 | Candidate SXA002 | Evidence / reviewer |
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

Sources: [Shenxin SXA002 product information](https://shenxinic.com/products), [ADI AD9434 product page and data sheet](https://www.analog.com/en/products/ad9434.html).

*AD9434 is a trademark of Analog Devices, Inc. SXA002 is an independently designed pin-to-pin alternative. All trademarks belong to their respective owners.*
