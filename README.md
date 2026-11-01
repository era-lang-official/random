# Era Random (`github.com/era-lang-official/random`)

Fast 64-bit pseudo-random number generator (PRNG) and Fisher-Yates array shuffling for Era.

## Features
- **Xorshift* 64-bit Engine**: High-period, zero-allocation random generation.
- **Range Generation**: `next_int_range(min, max)`.
- **String Generation**: Alphanumeric random tokens.
- **Fisher-Yates Shuffle**: In-place unbiased array shuffling.

## Usage
```era
import "github.com/era-lang-official/random";

fn main() {
    let mut rng = Rng::from_entropy();
    let roll = rng.next_int_range(1, 6);
    let token = rng.next_string(16);
}
```

