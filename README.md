# BBH-ja (日本語版BIG-Bench Hard)

BBH-jaは、BIG-Bench Hard ([Paper](https://arxiv.org/abs/2210.09261), [GitHub](https://github.com/suzgunmirac/BIG-Bench-Hard/)) を翻訳したベンチマークデータセットである。大規模言語モデルの日本語によるChain of Thought能力の評価に用いることを想定している。

評価に用いる問題 (`bbh-ja/`) とfew-shot exampleに用いるためのprompt (`cot-prompts/`) からなる。
`bbh-ja/`はsubjectごとにjsonlで保存されており、`input`に問題文、`target`に答えが保存されている。`cot-prompts/`はsubjectごとにyamlで保存されており、`input`に問題文、`target`にCoTを含む答えが保存されている。

翻訳には[PLaMo Translation Model](https://huggingface.co/pfnet/plamo-2-translate)を利用した。


BBH-ja is a Japanese translation of the BIG-Bench Hard benchmark dataset ([Paper](https://arxiv.org/abs/2210.09261), [GitHub](https://github.com/suzgunmirac/BIG-Bench-Hard/)). It is designed specifically for evaluating Japanese-language Chain of Thought capabilities in large language models.

The dataset consists of two components: evaluation problems (stored in `bbh-ja/`) and prompts for few-shot examples (stored in `cot-prompts/`).
`bbh-ja/` is organized by corpus subject and stored in JSON Lines format, with problem statements contained in `input` fields and correct answers stored in `target` fields. `cot-prompts/` is also organized by corpus subject but uses YAML format, with problem statements in `input` fields and answers containing Chain of Thought reasoning in `target` fields.

We used the [PLaMo Translation Model](https://huggingface.co/pfnet/plamo-2-translate) for translation.

Built with PLaMo

## Citation

If you use this repository, please cite this repository:

```
@misc{mikami2025-bbhja
    title={{BBH-ja}},
    year={2025},
    url = {https://github.com/pfnet-research/bbh-ja}
}
```
