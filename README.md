# Integrated Clock Gating (ICG) Cell Design using Microwind

## Why Clock Gating?
Clock gating solves this problem by:
- Disabling the clock signal for idle modules
- Reducing switching activity
- Lowering dynamic power consumption
- Improving overall power efficiency of the chip

---

### Working Principle
1. The **Enable (EN)** signal controls whether the clock should propagate.
2. The **Latch** samples the enable signal during the safe clock phase.
3. The output of the latch is connected to an **AND gate** with the clock.
4. If **EN = 1**, the clock passes through the AND gate.
5. If **EN = 0**, the clock is blocked.

This structure prevents **glitches in the clock signal**, which is critical for reliable digital system operation.

### Latch-AND Based ICG Cell


---

---

## Conclusion
The Integrated Clock Gating (ICG) cell is an effective technique used in modern VLSI systems to reduce dynamic power consumption. By implementing the latch-AND based architecture using the Microwind tool, this project demonstrates how clock gating can efficiently control clock propagation and improve power efficiency in digital circuits.
