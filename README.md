# MathBridge: A Large Corpus Dataset for Translating Spoken Mathematical Expressions into $LaTeX$ Formulae for Improved Readability 🧮

## Dataset
The MathBridge dataset is available on huggingface🤗.

- [MathBridge in huggingface🤗 dataset](https://huggingface.co/datasets/aaai25withanonymous/MathBridge)

## Fine-tuned Models
We have fine-tuned a range of models on the MathBridge. These models are available for download and use on Hugging Face.

### Available Models:
- **MathBridge T5 Small**: [huggingface🤗 model](https://huggingface.co/aaai25withanonymous/MathBridge_T5_small)
- **MathBridge T5 Base**: [huggingface🤗 model](https://huggingface.co/aaai25withanonymous/MathBridge_T5_base)
- **MathBridge T5 Large**: [huggingface🤗 model](https://huggingface.co/aaai25withanonymous/MathBridge_T5_large)
- **MathBridge BART Base**: [huggingface🤗 model](https://huggingface.co/aaai25withanonymous/MathBridge_BART_base)
- **MathBridge BART Large**: [huggingface🤗 model](https://huggingface.co/aaai25withanonymous/MathBridge_BART_large)
- **MathBridge mBART**: [huggingface🤗 model](https://huggingface.co/aaai25withanonymous/MathBridge_mBART)

#### Model Parameters:
<table style="width:50%; border-collapse:collapse; text-align:right;">
    <thead>
    <tr>
      <th style="border-bottom: 2px solid black; padding: 5px;"><strong>Model</strong></th>
      <th style="border-bottom: 2px solid black; padding: 5px; text-align:right;"><strong>Parameters</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border-bottom: 1px solid black; padding: 5px;">BART-base</td>
      <td style="border-bottom: 1px solid black; padding: 5px; text-align:right;">139 M</td>
    </tr>
    <tr>
      <td style="border-bottom: 1px solid black; padding: 5px;">BART-large</td>
      <td style="border-bottom: 1px solid black; padding: 5px; text-align:right;">406 M</td>
    </tr>
    <tr>
      <td style="border-bottom: 1px solid black; padding: 5px;">T5-small</td>
      <td style="border-bottom: 1px solid black; padding: 5px; text-align:right;">60.5 M</td>
    </tr>
    <tr>
      <td style="border-bottom: 1px solid black; padding: 5px;">T5-base</td>
      <td style="border-bottom: 1px solid black; padding: 5px; text-align:right;">223 M</td>
    </tr>
    <tr>
      <td style="border-bottom: 1px solid black; padding: 5px;">T5-large</td>
      <td style="border-bottom: 1px solid black; padding: 5px; text-align:right;">738 M</td>
    </tr>
    <tr>
      <td style="border-bottom: 1px solid black; padding: 5px;">mBART-large-50</td>
      <td style="border-bottom: 1px solid black; padding: 5px; text-align:right;">406 M</td>
    </tr>
    <tr>
      <td style="padding: 5px;">GPT-3.5</td>
      <td style="padding: 5px; text-align:right;">175 B</td>
    </tr>
  </tbody>
</table>


### Experiment Resluts:
<table>
  <tr>
    <th rowspan="2">Models</th>
    <th colspan="5">Original</th>
    <th colspan="5">MathBridge Enhanced</th>
  </tr>
  <tr>
    <th>BLEU (↑)</th>
    <th>sBLEU (↑)</th>
    <th>Rouge1 (↑)</th>
    <th>CER (↓)</th>
    <th>WER (↓)</th>
    <th>BLEU (↑)</th>
    <th>sBLEU (↑)</th>
    <th>Rouge1 (↑)</th>
    <th>CER (↓)</th>
    <th>WER (↓)</th>
  </tr>
  <tr>
    <td><strong>BART-base</strong></td>
    <td>0.29</td>
    <td>31.3</td>
    <td>0.64</td>
    <td>0.51</td>
    <td>0.68</td>
    <td>0.26</td>
    <td>38.7</td>
    <td>0.64</td>
    <td>0.42</td>
    <td>0.58</td>
  </tr>
  <tr>
    <td><strong>BART-large</strong></td>
    <td>0.29</td>
    <td>31.0</td>
    <td>0.61</td>
    <td>0.52</td>
    <td>0.69</td>
    <td>0.31</td>
    <td>35.2</td>
    <td>0.63</td>
    <td>0.48</td>
    <td>0.54</td>
  </tr>
  <tr>
    <td><strong>T5-small</strong></td>
    <td>0.12</td>
    <td>14.9</td>
    <td>0.39</td>
    <td>1.25</td>
    <td>1.35</td>
    <td>0.31</td>
    <td>38.4</td>
    <td>0.75</td>
    <td>0.35</td>
    <td>0.55</td>
  </tr>
  <tr>
    <td><strong>T5-base</strong></td>
    <td>0.05</td>
    <td>6.05</td>
    <td>0.21</td>
    <td>2.63</td>
    <td>2.53</td>
    <td>0.28</td>
    <td>36.6</td>
    <td>0.67</td>
    <td>0.50</td>
    <td>0.74</td>
  </tr>
  <tr>
    <td><strong>T5-large</strong></td>
    <td>0.04</td>
    <td>4.77</td>
    <td>0.20</td>
    <td>1.92</td>
    <td>1.95</td>
    <td><strong>0.36</strong></td>
    <td><strong>46.8</strong></td>
    <td><strong>0.82</strong></td>
    <td><strong>0.26</strong></td>
    <td><strong>0.49</strong></td>
  </tr>
  <tr>
    <td><strong>mBART-large-50</strong></td>
    <td>0.21</td>
    <td>16.9</td>
    <td>0.42</td>
    <td>0.90</td>
    <td>1.37</td>
    <td>0.24</td>
    <td>23.6</td>
    <td>0.59</td>
    <td>0.58</td>
    <td>0.74</td>
  </tr>
  <tr>
    <td><strong>GPT-3.5(w/o p)</strong></td>
    <td>0.24</td>
    <td>38.9</td>
    <td>0.77</td>
    <td>0.43</td>
    <td>0.55</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
  </tr>
  <tr>
    <td><strong>GPT-3.5(w/ p)</strong></td>
    <td>0.44</td>
    <td>52.3</td>
    <td>0.88</td>
    <td>0.19</td>
    <td>0.37</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
  </tr>
  <tr>
    <td><strong>Average</strong></td>
    <td>0.16</td>
    <td>17.4</td>
    <td>0.41</td>
    <td>1.28</td>
    <td>1.42</td>
    <td>0.29</td>
    <td>36.5</td>
    <td>0.68</td>
    <td>0.43</td>
    <td>0.60</td>
  </tr>
  <tr>
    <td><strong>Improvement</strong></td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>76.0%</td>
    <td>109.0%</td>
    <td>65.9%</td>
    <td>66.4%</td>
    <td>57.5%</td>
  </tr>
</table>
**Notes:** Evaluation of the performance of PLMs' original and MathBridge-enhanced responses using the test dataset. 'sBLEU' refers to sacreBLEU. The averages for the 'Original' column exclude GPT-3.5 Models.
