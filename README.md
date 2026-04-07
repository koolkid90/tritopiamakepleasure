# tritopiamakepleasure
Ideal RNG — live hash of the nanosecond. No state. No hack. No repetition.

What is this

This is not a random number generator.  
This is a witness of time.

Every nanosecond, the system captures a unique, unrepeatable event:
- high‑resolution time (nanoseconds)
- cryptographically strong noise (WebCrypto)
- jitter from the event loop
- memory & call stack entropy

This raw moment is compressed into a SHA‑256 hash — and immediately discarded.  
The next nanosecond — a new hash. Forever.

---

## Why it works

| Property | Explanation |
|----------|-------------|
| No state | nothing to capture, nothing to predict |
| Non‑linear | no formula can produce the next hash |
| Unhackable | no algorithm to reverse, only the flow of time |
| Infinite entropy | each hash is born from new physical/quantum noise 
