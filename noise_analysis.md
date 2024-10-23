# Noise Analysis in Quantum Circuits

This section explores the effects of noise in quantum circuits and addresses common questions related to quantum noise.

---

## 1. How does the noise affect the results?

Noise in quantum circuits causes decoherence and errors in the output. Here's a comparison of results with and without noise for `p1 = 0.01` and `p2 = 0.01`:

- **Without Noise**: Ideal quantum output is predictable, with all gates functioning as expected.
- **With Noise**: The addition of noise introduces errors, causing deviations in the output probabilities. Some states that were not present in the ideal case may appear due to noise.

_Visualizations:_
Plot results comparing noisy vs. non-noisy outputs.
  ![Plot visualization](https://github.com/Rachel-Eva/Noise-Model/blob/main/plot.png)


## 2. Is there a way to decrease the effect of noise?

Yes, several techniques can help reduce the impact of noise:

- **Quantum Error Correction (QEC)**: By encoding qubits into logical qubits, we can detect and correct errors.
- **Circuit Optimization**: Reducing the number of gates in the circuit can decrease the number of error sources.
- **Post-Processing Error Mitigation**: Techniques like **zero-noise extrapolation** can help mitigate errors after computation.

## 3. How does the number of gates used affect the results?

Each additional gate in a quantum circuit introduces potential noise, as physical gates are not perfect. Here's a breakdown:

- **Fewer Gates**: Less chance of errors as fewer operations are performed.
- **More Gates**: As the number of gates increases, the cumulative noise grows, introducing more errors into the final result.

<!--_Example Simulations:_
- Compare circuits with fewer and more gates, and show how the noise scales with each.-->
