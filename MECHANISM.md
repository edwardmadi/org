# Code4rena Mechanism

### Wardens

To incentivize wardens, C4 uses a unique scoring system with two primary goals: reward contestants for finding unique bugs and also to make the contest resistant to Sybil attack. A secondary goal of the scoring system is to encourage contestants to form teams and collaborate.

Contestants are given shares for bugs discovered based on severity, and those shares give the owner a pro rata piece of the pot:

- Low Risk shares: `1 * (0.9 ^ (findingCount - 1)) / findingCount`
- Med Risk shares: `3 * (0.9 ^ (findingCount - 1)) / findingCount`
- High Risk shares: `10 * (0.9 ^ (findingCount - 1)) / findingCount`

Each share is redeemable for: `pot / number of shares`

### Judges

Judges are incentivized to review findings and determine allocation of the prize pool by receiving a share of the prize pool themselves.
