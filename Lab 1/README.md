# Lab 1 — Spectral Analysis of Deterministic Signals

The solutions for **Task 1, all 15 variants** from `Lab1_EN.pdf` are implemented in English in a Jupyter Notebook.

## Contents

- `Lab1_All_15_Variants.ipynb` — runnable notebook for all 15 variants with full K/W matrices, synthesized samples, 3 plots per variant, and validation using NumPy FFT.
- `requirements.txt` — Python dependencies.

## Running the notebook

```bash
python -m pip install -r requirements.txt
jupyter notebook Lab1_All_15_Variants.ipynb
```

Then use **Kernel → Restart & Run All** to create all numerical results and plots.

## Mathematics

For a spectrum of length `N`, the integer matrix is `K[k, mu] = k * mu`, the Fourier synthesis matrix is `W = exp(+2j*pi*K/N)`, and the IDFT is calculated using matrix multiplication: `x = W @ X / N`. The separate call to `numpy.fft.ifft` verifies the result rather than performing the synthesis.

The provided spectra generally generate complex-valued time-domain signals, so the plots show real, imaginary and magnitude components.

Some task variants duplicate one another (1=3=11=13, 2=12, 4=14, 5=15); every numbered variant is nevertheless included.

## PDF deliverables

The standalone report (`Lab1_Report.pdf`) and the result/plot PDF (`Lab1_Notebook_Export.pdf`) were generated separately and can be downloaded from the corresponding ChatGPT conversation. They are not stored in this GitHub folder.
