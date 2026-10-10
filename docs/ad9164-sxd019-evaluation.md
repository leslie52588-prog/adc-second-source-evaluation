# AD9164 → SXD019: existing-board evaluation worksheet

**Status:** Public blank method. No measured data or customer board claim.

## Scope

Shenxin lists SXD019 as a pin-to-pin candidate for the AD9164 BGA169 package. ADI lists AD9164 in **BGA165 and BGA169** variants — verify the fitted package before applying any equivalence; SXD019 is BGA169 only (11 × 11 × 2 mm). SXD019 is a 16-bit DAC up to 12 GSPS in 2× NRZ mode (first Nyquist zone); NRZ / Mix-Mode / RZ modes run to 6 GSPS. Package thickness (2 mm) and thermal ratings differ from AD9164 — confirm mechanical fit and thermal design separately. A pin match is the beginning of the evaluation, not a system qualification.

## 1. Establish the baseline

| Item | Reference AD9164 | Candidate SXD019 | Evidence / reviewer |
|---|---|---|---|
| Full populated ordering code and package (BGA165 vs BGA169) | TBD | TBD | TBD |
| PCB revision, fitted options, assembly lot | TBD | TBD | TBD |
| Supply, clock source (≤ 6 GHz) and jitter conditions | TBD | TBD | TBD |
| SPI/register configuration, NCO FTW width (48-bit) | TBD | TBD | TBD |
| Output mode (NRZ / Mix / RZ), Nyquist zone, full-scale current (8–40 mA) | TBD | TBD | TBD |

## 2. Verify the JESD204B link

Record lane count (up to 8), per-lane rate (≤ 10 Gbps, per official SXD019 product spec), subclass, LMFC alignment, SYNC behavior and link test patterns (CGS / ILA / JTSPAT). A locked link checks the digital path; it does not demonstrate analog or system performance.

| Item | Reference | Candidate | Pass criterion |
|---|---|---|---|
| Lane rate, subclass and LMFC alignment | TBD | TBD | TBD |
| Link establishment and re-sync behavior | TBD | TBD | TBD |
| Test-pattern integrity across all lanes | TBD | TBD | TBD |

## 3. Check the datapath configuration

Record interpolation factor (1/2/3/4/6/8/12/16/24×), inverse-sinc setting, NCO frequency word and target Nyquist zone for each operating mode. Confirm the 12 GSPS rate is only used in 2× NRZ mode.

| Item | Reference | Candidate | Pass criterion |
|---|---|---|---|
| Interpolation chain and inverse-sinc FIR | TBD | TBD | TBD |
| NCO setting vs. target output zone | TBD | TBD | TBD |
| Mode-dependent update-rate limits | TBD | TBD | TBD |

## 4. Repeat the instrument's acceptance test

Use the instrument's own release procedure — for 5G/base-station, wireless or test-equipment builds, the applicable SFDR/IMD masks, channel flatness and temperature range. Record the same clock, output network, load and software build for each device. Do not publish customer limits or controlled data.

| Test | Reference result | Candidate result | Limit / disposition |
|---|---|---|---|
| SFDR / IMD under instrument conditions | TBD | TBD | TBD |
| Output flatness across the band of interest | TBD | TBD | TBD |
| Temperature / repeated build if required | TBD | TBD | TBD |

## Handoff

The result is meaningful only with a board revision, test date, setup, owner and sign-off. Contact Leslie at **gjr@shenxinic.com** with the full fitted part code and board revision for the applicable pin comparison and sample discussion.

Sources: [Shenxin SXD019 product information](https://shenxinic.com/products), [ADI AD9164 product page and data sheet](https://www.analog.com/en/products/ad9164.html).

*AD9164 is a trademark of Analog Devices, Inc. SXD019 is an independently designed pin-to-pin alternative. All trademarks belong to their respective owners.*
