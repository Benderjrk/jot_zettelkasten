# Wasmtime Reaches 1.0: Fast, Safe and Production Ready!

> Notes from [Lin Clark](https://bytecodealliance.org/articles/wasmtime-1-0-fast-safe-and-production-ready)

As of today, the Wasmtime WebAssembly runtime is now at 1.0! this means
that all of us in the Bytecode Alliance agree that it is fully ready to
use in production.

In truth, we could have called Wasmtime production-ready [more than a
year
ago.](https://github.com/bytecodealliance/rfcs/pull/14#issuecomment-915589031)
But we didn't want to release just any WebAssembly engine. We wanted to
have a super fast and super safe WebAssembly engine. We wanted to feel
really confident with we recommend that people choose Wasmtime.

So to make sure it's production ready for all of you, a number of us in
the Bytecode Alliance have been running Wasmtime in production ourselves
for the past year. And Wasmtime has been doing great in these production
environments, providing a stable platform while also giving us security
and speed wins.

![vetting wasmtime in
production](../../images/wasmtime_1.0/prod-timeline.png)

Here are some of our experiences with the new, improved Wasmtime:

* **Shopify -- 14 months in production**
  - Shopify switched to Wasmtime for another WebAssembly engine in July 2021. With the switch, Shopify saw an `average execution performace improvements of ~50%.`

* **Fastly -- 6 months in production**
  - Fastly switched to Wasmtime from another WebAssembly engine in March
    2022. Fastly also saw a `~50% improvement in execution time`. In
          addition, Fastly saw a `72% to 163% increase in
          requests-per-second` it could serve. Fastly has since served
          `trillions of request` using Wasmtime.

* **DFINITY -- 16 months in production**
  - DFINITY launched the Internet Cimputer blockchain using Wasmtime in
    May 2021. Since then, the Internet Computer has executed `1
    quintillion (10^18) instructions for over 150,000 smart contracts`
    without any production issues.

* **InfinyOn -- 14 months in production**
  - InfinyOn Cloud has been using Wasmtime in production since July
    2021. With Wasmtime, InfinyOne has been able to deliver a greater
          than `5x throughput improvement in end-to-end stream
          processing` when compared to Java-based platforms like Kafka.


































