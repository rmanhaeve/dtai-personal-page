---
layout: about
permalink: /

profile:
  align: right
  image: prof_pic.jpg
  address: >
    <p>Departement Computerwetenschappen,</p>
    <p>Celestijnenlaan 200A,</p>
    <p>3001 Leuven</p>

news: true
social: true
---

Hi, I'm {{ site.first_name }} {{ site.last_name }}, a postdoctoral researcher in the <a href="https://dtai.cs.kuleuven.be/" target="_blank">DTAI</a> research group at <a href="https://www.kuleuven.be/kuleuven/" target="_blank">KU Leuven</a>. I work on neurosymbolic AI (NeSy): combining the learning of neural networks with logical and probabilistic reasoning.

My current work is on <a href="https://wms.cs.kuleuven.be/cs/onderzoek/deeplog" target="_blank">DeepLog</a>, a framework that provides common building blocks for neurosymbolic AI. It abstracts over the kind of logic used (Boolean, fuzzy or probabilistic) and over whether the logic sits in the model's architecture or in its loss function, so that a wide range of existing NeSy systems can be expressed, compared and run on a GPU with the same parts. I am the lead developer of its software framework.

During my PhD I developed DeepProbLog, which extends the probabilistic logic programming language ProbLog with neural predicates: facts whose probabilities are computed by a neural network. With colleagues I also wrote a survey that relates neurosymbolic AI to statistical relational AI, and we teach tutorials on both; see <a class="page-link" href="{{ '/presentations/' | prepend: site.baseurl | prepend: site.url }}">presentations</a>.

### Software

- [DeepLog](https://github.com/ML-KULeuven/deeplog): a Python library on top of PyTorch for building neurosymbolic systems ([documentation](https://dtai.cs.kuleuven.be/deeplog/)).
- [DeepProbLog](https://github.com/ML-KULeuven/deepproblog): neural probabilistic logic programming, built on ProbLog.

### Selected publications

- R. Manhaeve, S. Colamonaco, V. Derkinderen, R. Adriaensen, L. Van Praet, L. De Raedt and G. Marra. [*DeepLog: A Software Framework for Modular Neurosymbolic AI*](https://arxiv.org/abs/2605.10279). IJCAI-ECAI 2026, demonstrations track.
- V. Derkinderen\*, R. Manhaeve\*, R. Adriaensen, L. Van Praet, L. De Smet, G. Marra and L. De Raedt. [*The DeepLog Neurosymbolic Machine*](https://arxiv.org/abs/2508.13697). arXiv, 2025. (\* shared first authors)
- G. Marra, S. Dumančić, R. Manhaeve and L. De Raedt. [*From Statistical Relational to Neurosymbolic Artificial Intelligence: a Survey*](https://doi.org/10.1016/j.artint.2023.104062). Artificial Intelligence, 2024.
- R. Manhaeve, S. Dumančić, A. Kimmig, T. Demeester and L. De Raedt. [*Neural Probabilistic Logic Programming in DeepProbLog*](https://doi.org/10.1016/j.artint.2021.103504). Artificial Intelligence, 2021.
- R. Manhaeve, S. Dumančić, A. Kimmig, T. Demeester and L. De Raedt. [*DeepProbLog: Neural Probabilistic Logic Programming*](https://proceedings.neurips.cc/paper/2018/hash/dc5d637ed5e62c36ecb73b654b05ba2a-Abstract.html). NeurIPS 2018, spotlight.

The full list is on the <a class="page-link" href="{{ '/lirias/' | prepend: site.baseurl | prepend: site.url }}">publications</a> page. You can find more information on my <a class="page-link" href="{{ site.ku_leuven_personnel_number | prepend: 'https://www.kuleuven.be/wieiswie/en/person/0' }}">KU Leuven who's who page.</a>
