Hilbert–Kunz theory of diagonals and Han–Monsky theory
======================================================

In this repo, you can find Jupyter notebooks in Sagemath to compute Hilbert–Kunz functions, multiplicities and F-signatures of diagonal hypersurfaces via Han–Monsky and Chiang–Hung algorithm. It comes with some quick notes on the theory, with code snippets embedded. 

This notebooks were hugely improved by Claude Opus 5.5, using old code I developed during my dissertation.

If you cannot run it locally, click the button below to open a Binder environment to interact with these Jupyter Notebooks. In this case, have in mind that the launch of the Binder usually takes between one and two minutes.

.. image:: https://mybinder.org/badge_logo.svg
 :target: https://mybinder.org/v2/gh/joelcrey/JupyterNotebooks/HEAD?urlpath=tree


The Jupyter Notebooks
_____________________
All the notebooks are in the folder 'notebooks'. The notebooks 01, 02 and 03 use the module 'hilbert_kunz.py', which must be in the same folder. They follow the notes 'han_monsky.pdf' [Notes].

1. **Representation ring.** The notebook '01_representation_ring.ipynb' allows you to compute in the Han–Monsky ring (or representation ring) [HM93]: products of deltas and lambdas, changes of basis between them, and Yoshida's matrix representation.

2. **Diagonal hypersurfaces: HK and F-signature functions.** The notebook '02_han_monsky.ipynb' allows you to compute the Hilbert–Kunz function, Hilbert–Kunz multiplicity, F-signature function and F-signature of any hypersurface of the form x_1^d_1+...+x_n^d_n for any fixed characteristic p, via the Han–Monsky algorithm [HM93]. The main functions are HK_function_diagonal(f) and FS_function_diagonal(f).

3. **Sums of monomials in disjoint variables: HK functions.** The notebook '03_chiang_hung.ipynb' implements Chiang and Hung's algorithm to compute the Hilbert–Kunz function and multiplicity of any hypersurface of the form (x_(1,1)...x_(1,d_1))^e_1+...+(x_(m,1)...x_(m,d_m))^e_m (i.e., sum of monomials of disjoint variables; in particular, diagonal hypersurfaces). The main function is HK_function_disjoint_monomials(f). *Disclaimer:* The function in this notebook was not implemented by me; it was written entirely by Claude after being prompted to implement the algorithm developed by Chiang and Hung in their 1998 paper [CH98], so I claim no correctness of the algorithm as of yet; however, it checks out in all cases from [CH98] I could try, and also with numerical experiments for first values of the Hilbert–Kunz functions of several other hypersurfaces.

4. The notebook 'hanmonskyalgorithm.ipynb' is my original implementation of Han and Monsky's setup and algorithm from Han and Monsky's paper [HM93] and Yoshida's notes [Yo09], before asking Claude to improve it. It computes the Hilbert–Kunz multiplicity of any diagonal hypersurface (eHK_diagonal(p,[e_0,...,e_d])) and the Hilbert–Kunz function of any diagonal hypersurface (HK_diagonal(p,[e_0,...,e_d])). Everything that Claude did is based on this.

References
____________________
[Notes] Castillo-Rey, J. The Hilbert–Kunz function and F-signature function of the diagonal hypersurfaces. Notes ('notebooks/han_monsky.pdf').

[CH98] Chiang, L., & Hung, Y. C. (1998). On Hilbert-Kunz functions of some hypersurfaces. Journal of Algebra, 199(2), 499-527.

[HM93] Han, C., & Monsky, P. (1993). Some surprising Hilbert-Kunz functions. Mathematische Zeitschrift, 214(1), 119-135.

[Yo09] Yoshida, K. (2009). Small Hilbert-Kunz multiplicity and (A_1)-type singularity. Proceedings of the 4th Japan-Vietnam Joint Seminar on Commutative Algebra by and for Young Mathematicians, Meiji University, Japan.

The full list of references is at the end of each notebook.
