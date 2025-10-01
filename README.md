<div align="center" style="font-family: charter;">
<h1>TFPI: Thinking-Free Policy Initialization Makes Distilled Reasoning Models More Effective and Efficient Reasoners</br></h1>


<a href="" target="_blank">
    <img alt="arXiv" src="https://img.shields.io/badge/arXiv-TFPI-red?logo=arxiv" height="20" /></a>
<a href="" target="_blank">
    <img alt="" src="https://img.shields.io/badge/%F0%9F%A4%97%20_Model-TFPI-ffc107?color=ffc107&logoColor=white" height="20" /></a>

<div>
    <a href="https://xinxu-ustc.github.io/" target="_blank">Xin Xu</a><sup>1,</sup><sup>2,</sup>,</span>
    <a href="" target="_blank">Cliveb AI</a><sup>1</sup>,</span>
    <a href="https://github.com/yk7333" target="_blank">Kai Yang</a><sup>1,</sup>,</span>
    <a href="https://github.com/dandingsky" target="_blank">Tianhao Chen</a><sup>2,</sup>,</span>
    <a href="https://www.presidentsoffice.hku.hk/leadership/professor-yang-wang" target="_blank">Yang Wang</a><sup>3,</sup>,</span>
    <a href="https://github.com/yangsaiyong" target="_blank">Saiyong Yang</a><sup>1,</sup>,</span>
    <a href="https://sites.google.com/site/eeyangc/" target="_blank">Can Yang</a><sup>2,</sup>,</span>
</div>

<div>
    <sup>1</sup>Hunyuan, Tencent&emsp;
    </br>
    <sup>2</sup>The Hong Kong University of Science and Techology&emsp;
    </br>
    <sup>3</sup>The University of Hong Kong&emsp;
    </br>
</div>


</div>      

## 📝 News
- [2025/9/30] We released the [paper](https://arxiv.org/abs/2509.26226) and [temporary repo](https://github.com/XinXU-USTC/TFPI-temp) !

## Reproduction

**This is a temporary repository. Our code and training checkpoints are currently undergoing an audit in accordance with Tencent's regulations.**
For now, to reproduce our results, you can perform TFPI training using [VeRL](https://github.com/volcengine/verl) codebase by modifying `utils/datasets/rl_dataset.py`:

```Python
raw_prompt = self.tokenizer.apply_chat_template(messages, add_generation_prompt=True, tokenize=False)
# added codes
raw_prompt += "<think>\n\n</think>\n\n"
```
For evaluation, you could refer to [DeepScaler](https://github.com/agentica-project/rllm) and [IFEval evaluation](https://github.com/google-research/google-research/tree/master/instruction_following_eval).


## ✏️ Citation

### Bib
If you find TFPI useful for your research and applications, please cite using this BibTeX:
```

```
