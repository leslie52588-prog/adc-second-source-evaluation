# AD9253 → JXA036: existing-board evaluation worksheet

**Status:** Public blank method. No measured data or customer board claim.

## Scope

Shenxin lists JXA036 as a pin-to-pin candidate for the matching AD9253 48-pin package. The JXA036 listing describes 14-bit, four-channel, 125 MSPS operation. ADI lists AD9253 orderable 80/105/125 MSPS versions. Verify the complete ordering suffix, speed grade, package and configuration; do not infer qualification of every variant from a family name.

## 1. Establish the baseline

| Item | Reference AD9253 | Candidate JXA036 | Evidence / reviewer |
|---|---|---|---|
| Full populated ordering code and package | TBD | TBD | TBD |
| PCB revision, fitted options, assembly lot | TBD | TBD | TBD |
| Supply, reference and input full-scale configuration | TBD | TBD | TBD |
| Sample clock source, rate and jitter conditions | TBD | TBD | TBD |
| SPI/register configuration and power-down states | TBD | TBD | TBD |

## 2. Verify digital capture

Record serial LVDS output mode, DCO and FCO relationship, FPGA bitstream, capture timing and any test-pattern procedure. A passing test pattern checks the data path; it does not demonstrate analog or instrument performance.

| Item | Reference | Candidate | Pass criterion |
|---|---|---|---|
| DCO/FCO capture and framing | TBD | TBD | TBD |
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

Sources: [Shenxin JXA036](https://shenxinic.com/product/jxa036), [ADI AD9253](https://www.analog.com/en/products/ad9253.html).
