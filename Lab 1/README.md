# Lab 1 — Spectral Analysis of Deterministic Signals

The solutions for all 15 variants use a Jupyter Notebook and matrix-based IDFT.

## Method

For each spectrum `X`, the integer outer-product matrix `K` and Fourier matrix `W = exp(2j*pi*K/N)` are constructed, then `x = W @ X / N` is calculated. The result is verified against `numpy.fft.ifft`, and the real part, imaginary part and magnitude of the signal are plotted.

## Files

- `Lab1_All_15_Variants.ipynb` — all 15 variants, matrices K and W, calculations and figures.
- `Lab1_Report.pdf` — English report.
- `Lab1_Notebook_Export.pdf` — PDF of all variant results and plots.
- `requirements.txt` — dependencies.

Run with `python -m pip install -r requirements.txt` and then `jupyter notebook Lab1_All_15_Variants.ipynb`.
