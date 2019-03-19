## Dual-Kernel Online Reconstruction of Power Maps
We present a measurement-driven algorithm to map
the large-scale channel losses observed between a cellular base
station and any point in its coverage area. The algorithm
is on-line, meaning that it operates on continuously arriving
measurements. Its distinguishing features are the use of two
kernel functions, suitably chosen for the problem at hand, and
a simple technique to sparsify the dictionary of measurements
retained in memory. Evaluations in campus and urban settings
indicate that the proposed algorithm reduces, roughly in half,
the prediction error of existing single-kernel and multikernel
algorithms.

### Conclusion
A clean separation of the DC component from the rest
of the large-scale losses, via two suitable kernel functions,
benefits the online reconstruction of large-scale loss maps. The
accuracy increases with respect to the single-kernel version,
but also with respect to a multikernel solution. This confirms
that the number of kernels should be chosen carefully to
match the structure of the problem, and adding unnecessarily
many kernels may end up being detrimental. With two kernels,
the performance approaches the baseline represented by more
complex batch schemes, where, rather than a limited-size
dictionary, all measurements must be stored.
To reinforce the above insight it is worth mentioning that,
in Section VI, the dual-kernel approach has been run with
the parameter q (which, recall, indicates the number of recent
measurement over which APSM projects at every step) set to
q = 1, and yet this has sufficed to outperform the single-kernel
result, which has been run with q = 20. This confirms the
effectiveness of the DC kernel at tracking the map’s average,
something that without a DC kernel requires a larger value of
q and therefore higher complexity.

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/RasoulNik/RasoulNik/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
