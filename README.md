# suffix_trees
Python implementation of Suffix Trees and Generalized Suffix Trees. Also provided methods with typcal applications of STrees and GSTrees. 

### Installation

```bash
pip install suffix-trees
```

### Usage

```python
from suffix_trees import STree

# Suffix-Tree example.
st = STree.STree("abcdefghab")
print(st.find("abc")) # 0
print(st.find_all("ab")) # [0, 8]

# Generalized Suffix-Tree example.
a = ["xxxabcxxx", "adsaabc", "ytysabcrew", "qqqabcqw", "aaabc"]
st = STree.STree(a)
print(st.lcs()) # "abc"

# Generalized Suffix-Tree example with multiple lcs equal sized
a = ["klexxxabc", "kleyyyabc"]
st = STree.STree(a)
print(st.lcsm()) # ["kle", "abc"]
```
