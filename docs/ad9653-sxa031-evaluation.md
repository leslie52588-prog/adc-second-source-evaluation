# AD9653 → SXA031: existing-board evaluation worksheet

**Status:** Public blank method. No measured data or customer board claim.

## Scope

Shenxin lists SXA031 as a pin-to-pin candidate for the matching AD9653 package. The SXA031 listing describes 16-bit, four-channel, 125 MSPS operation. Verify the complete ordering suffix, speed grade, package and configuration; do not infer qualification of every variant from a family name.

## 1. Establish the baseline

| Item | Reference AD9653 | Candidate SXA031 | Evidence / reviewer |
|---|---|---|---|
| Full populated ordering code and package | TBD | TBD | TBD |
| PCB revision, fitted options, assembly lot | TBD | TBD | TBD |
| Supply, reference and input full-scale configuration | TBD | TBD | TBD |
| Sample clock source, rate and jitter conditions | TBD | TBD | TBD |
| SPI/register configuration and power-down states | TBD | TBD | TBD |

## 2. Verify digital capture

Record serial output mode, clock/data relationship, FPGA bitstream, capture timing and any test-pattern procedure. A passing test pattern checks the data path; it does not demonstrate analog or instrument performance.

| Item | Reference | Candidate | Pass criterion |
|---|---|---|---|
| Clock/data capture and framing | TBD | TBD | TBD |
| Four-channel data integrity and alignment | TBD | TBD | TBD |
| Restart and operating-mode transitions | TBD | TBD | TBD |

## 3. Repeat the instrument's acceptance test

For medical ultrasound, use the manufacturer's approved phantom and image-quality release procedure. For industrial NDT, use the approved reference block or inspected specimen and the instrument's stated limits. Record the same input chain, gain, filter, software build, stimulus and environment for each device. Do not publish patient data or customer limits.

| Test | Reference result | Candidate result | Limit / disposition |
|---|---|---|---|
| Relevant analog noise / dynamic range | TBD | TBD | TBD |
| Channel-to-channel consistency | TBD | TBD | TBD |
| System-level image or detection test | TBD | TBD | TBD |
| Temperature / repeated build if required | TBD | TBD | TBD |

## Handoff

The result is meaningful only with a board revision, test date, setup, owner and sign-off. A pin match is the beginning of the evaluation. Contact Leslie at **gjr@shenxinic.com** for the matching pin comparison and sample discussion.

Sources: [Shenxin SXA031 product information](https://shenxinic.com/products), [ADI AD9653 product page and data sheet](https://www.analog.com/en/products/ad9653.html).

*AD9653 is a trademark of Analog Devices, Inc. SXA031 is an independently designed pin-to-pin alternative. All trademarks belong to their respective owners.*
