---
title: 'Hello, World!'
date: 2023-11-19T15:00:00.000Z
draft: false
---

## Hello World!

Hi!

```rust
use peroxide::fuga::*;

fn main() {
    let x = seq(1, 10, 1);
    let y = x.fmap(|t| t.powi(2));
    
    let cs = cubic_hermite_spline(&x, &y, Akima);
    let x_new = seq(1, 10, 0.1);
    let y_new = cs.eval_vec(&x_new);
    y_new.print();
}
```

$$ \mathcal{L} = \frac{1}{2} mv^2 $$
