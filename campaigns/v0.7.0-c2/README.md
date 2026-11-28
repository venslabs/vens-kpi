# Campaign 2: vens v0.7.0 against v0.6.0

Under [`vens-kpi/1.0`](../../spec/1.0/vens-kpi-1.0.md) (tag `spec-1.0`, sha256 `876bac7ea5d4fa37a3810b91af8acdd138c059f7d2ea92070a6d3bddffeaa763`).

## Status

**Frozen, signed by both reviewers and approved by the maintainer on 2026-11-28; not started.** Published before the first run (spec §6): the frozen file, the reader's hash and the commitments of fresh sealed data. Campaign 1 ended after stage 1, repetition 1, with no verdict: its spend gate failed on a ceiling F0 had set wrong. Its sets count as read, so campaign 2 uses new ones. What changed and why is in [`F0.md`](F0.md) §0.

## Frozen before the first run

| Item | Value |
|---|---|
| Candidate | venslabs/vens#436 at `34ef2a1a614bca71f90042c9865fdf275704f1ee`, darwin/arm64 binary sha256 `47155d4bbb67177c613b205b4b54b001e29577a8f6a60921869f68208f771cda` |
| R | v0.6.0 release asset `vens-v0.6.0-darwin-arm64.tar.gz`, cosign-verified, binary sha256 `da3c2daa19661bdd518066f56a1f4269315570db1bebef635be17cedc653d461` |
| Models | `claude-sonnet-4-6`, `gpt-5.4-mini-2026-03-17` |
| Reader | sha256 `41f84b99cfdaad7c26923b24f4a60d86253b06271b64139bcf9700bb339495de`; config `14c37ae772a7b9b437d2c98ae816f9fa6728d4426eaa572500b5d3dea1fc5831` |
| Frozen file | [`F0.md`](F0.md), sha256 `10f72a96370a5e7f30e343d8670287bee1f76483eebba89c1527d3910d6ed771` |
| Spend cap | $272.02 ($300 for v0.7.0 less campaign 1's $27.98), in stages with a go from the maintainer at each one |

## Commitments

Salted SHA-256 commitments in [`commitments/`](commitments/); salts and sets stay private until retirement.

| Set | Aggregate |
|---|---|
| `sealed-v0.7.0-c2`: 92 CVEs + 4 sentinels, 3 fresh contexts | `aa62cbc93bcdf3ac222754354eab70f06d3fb9b009a05677b09f2b7d14cd344d` |
| `dir-v0.7.0-c2`: 100 context-sensitivity pairs and 20 controls | `1f7f20db5f30fce71cb915ddaff9b2eca0561def40566cb11f540fc78c94577a` |
| `inv-prep-v0.7.0-c2.r2`: input-invariance rules and tools | `2cbcd0e721622f304b95d807a0848acd50df127f7e61f72e69662c03ed08bc5d` |
| `inv-data-v0.7.0-c2`: 26 bases, paraphrases and planted variants | `caebfb296626d0829f034051ce3dbe8d0739bab284811a2743e2f32617aed37a` |
| `frame-v0.7.0-c2`: the population drawn from, campaign 1's read set and its families excluded | `01f0b77bcc1673b21c20075b2c123f3dfb50c767ae725d88a7dbf41d5f0a3880` |

Drawn with drand quicknet round 34354212 (2026-11-28T11:40:00Z), randomness `6ba751d7a47e9a6d8dec9535fe55dc13c821da4cd36913dffd608d2e9a5625bd`, under a policy committed before the round (sha256 `7bdc48b29e87a63f85d9cd0ffb64a4506f06851b7ef222a00c3976e2e574f771`). The set is 92 CVEs, not 100: without campaign 1's set and families, the 20 images held no v4-only CVE and 2 UNKNOWN ones, a shortfall recorded before the draw.

## After the campaign

Added here: the reading at the stage reached, the calibration, every attempt and result under opaque aliases, the spend charged and the delivery decision.
