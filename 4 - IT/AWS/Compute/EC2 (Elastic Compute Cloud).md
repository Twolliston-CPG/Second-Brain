The problem: buying, racking, and maintaining physical servers is slow and expensive, and you have to guess your capacity years ahead. EC2 gives you virtual servers on demand, in minutes, that you can resize or throw away. You still manage the operating system, patching, scaling, and software, but the hardware is gone from your list.

_Instance types_ address the fact that workloads need different shapes of hardware. Families are tuned for general purpose (M, T), compute-heavy work (C), memory-heavy work (R, X), storage-heavy work (I, D), and GPU or accelerator work (P, G, Inf, Trn). Picking the right type means you don't pay for resources you don't use.

_Pricing models_ address the fact that workloads have different cost and commitment profiles:

- **On-Demand**: pay by the second with no commitment. It is the most flexible and most expensive option, so it suits unpredictable or short-lived workloads.
- **Spot**: uses spare AWS capacity at up to about 90% off, but AWS can take the instance back with a two-minute warning. It suits fault-tolerant jobs like batch processing, CI builds, and rendering.
- **Reserved Instances**: commit to a specific instance configuration for 1 or 3 years for a large discount. They suit steady, predictable workloads like a database that always runs.
- **Savings Plans**: commit to a dollar amount of compute per hour for 1 or 3 years instead of a specific instance. You get similar discounts with more flexibility, and Compute Savings Plans also apply to Fargate and Lambda.