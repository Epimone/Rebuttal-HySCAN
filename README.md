# Rebuttal-HySCAN
**Table 1: Certified accuracy (%) of HySCAN and HyCAS on ImageNet.**
| Method | sigma | r=0.00 | r=0.25 | r=0.50 | r=0.75 | r=1.00 | r=1.25 | r=1.50 | r=2.00 |
|:--|:--:|--:|--:|--:|--:|--:|--:|--:|--:|
| HyCAS | 0.25 | 72.3 | 63.9 | 55.6 | 46.4 | 40.7 | 35.2 | 29.7 | 5.42 |
| HyCAS | 0.50 | 69.2 | 60.6 | 53.9 | 45.6 | 41.1 | 36.3 | 32.7 | 24.8 |
| HyCAS | 1.00 | 53.8 | 50.4 | 47.5 | 39.2 | 36.6 | 32.3 | 29.1 | 25.3 |
| HyCAS | 1.50 | 39.2 | 37.9 | 34.9 | 32.8 | 30.1 | 28.7 | 27.5 | 26.4 |
| HySCAN | 0.25 | 71.9 | 65.2 | 56.7 | 47.9 | 42.3 | 37.1 | 30.7 | 7.15 |
| HySCAN | 0.50 | 68.9 | 61.5 | 55.1 | 46.8 | 42.3 | 37.4 | 33.9 | 26.2 |
| HySCAN | 1.00 | 53.5 | 50.4 | 47.9 | 40.7 | 38.1 | 34.7 | 31.5 | 28.2 |
| HySCAN | 1.50 | 39.2 | 38.3 | 35.8 | 33.7 | 31.2 | 30.1 | 28.9 | 28.1 |

**Table 2: Certified accuracy (%) of HySCAN and HyCAS on CIFAR-10.**
| Method | sigma | r=0.00 | r=0.25 | r=0.50 | r=0.75 | r=1.00 | r=1.25 | r=1.50 | r=2.00 |
|:--|:--:|--:|--:|--:|--:|--:|--:|--:|--:|
| HyCAS | 0.25 | 85.4 | 70.1 | 56.7 | 44.3 | 36.5 | 29.6 | 22.9 | 8.52 |
| HyCAS | 0.50 | 80.7 | 65.3 | 54.8 | 44.3 | 36.8 | 30.3 | 23.4 | 12.5 |
| HyCAS | 1.00 | 64.9 | 60.6 | 53.1 | 43.7 | 36.6 | 31.5 | 25.1 | 20.3 |
| HyCAS | 1.50 | 48.5 | 44.8 | 37.6 | 34.3 | 30.1 | 27.8 | 25.6 | 21.5 |
| HySCAN | 0.25 | 85.2 | 70.4 | 57.3 | 45.5 | 37.9 | 30.7 | 24.1 | 9.94 |
| HySCAN | 0.50 | 80.3 | 66.4 | 56.1 | 45.8 | 38.3 | 31.7 | 25.1 | 13.9 |
| HySCAN | 1.00 | 64.9 | 61.2 | 55.2 | 46.4 | 39.7 | 34.8 | 29.3 | 25.1 |
| HySCAN | 1.50 | 48.3 | 45.5 | 39.4 | 36.7 | 33.4 | 30.1 | 28.3 | 25.7 |

Table 3: Empirical robustness (%) of HyCAS, DCS, RPF, CTRW, & HySCAN under EOT-PGD & adaptive attacks (BPDA and BPDA+EOT) on NIH-CXR and CIFAR-10.
| Pipeline | NIH-CXR@EOT-PGD | NIH-CXR@BPDA | NIH-CXR@ BPDA+EOT | CIFAR-10@ EOT-PGD |CIFAR-10@ BPDA | CIFAR-10@ BPDA+EOT |
| - | -: | -: | -: | -: | -: | -: |
| HyCAS | 83.59 | 82.24 | 78.31 | 68.38 | 68.12 | 66.50 |
| DCS | 81.14 | 76.72 | 74.93 | 69.81 | 69.30 | 67.56 |
| RPF | 82.22 | 77.34 | 75.28 | 66.12 | 67.94 | 65.41 |
| CTRW | 81.14 | 76.72 | 74.93 | 68.75 | 69.42 | 67.37 |
| HySCAN | 88.30 | 85.26 | 84.45 | 73.24 | 73.70 | 72.85 |

Table 4: base model vs base model comparison under same fraemworks ( Note: IN = ImageNet, C10= CIFAR-10)
| Pipeline  | (\sigma=.25) C10@.50 | C10@.75 | IN@.50 | IN@.75 | (\sigma=.50) C10@.50 | C10@.75 | IN@.50 | IN@.75 |
| - | -: | -: | -: | -: | -: | -: | -: | -: |
| Vanilla+RS | 43.4 | 26.1 | 0.0 | 0.0 | 41.3 | 32.4 | 36.8 | 28.7 |
| RPF+RS | 51.6 | 33.9 | 38.5 | 26.7 | 50.3 | 38.8 | 47.4 | 37.5 |
| CTRW+RS | 52.7 | 36.2 | 42.3 | 30.8 | 52.5 | 40.3 | 50.7 | 40.2 |
| HySCAN+RS | 57.3 | 45.5 | 56.7 | 47.9 | 56.1 | 45.8 | 55.1 | 46.8 |
| Vanilla+ARS | 51.4 | 39.1 | 52.7 | 43.1 | 50.2 | 38.9 | 50.3 | 43.4 |
| RPF+ARS | 53.0 | 40.5 | 53.5 | 43.5 | 51.7 | 42.3 | 48.5 | 39.9 |
| CTRW+ARS | 54.5 | 42.0 | 54.5 | 44.5 | 53.9 | 44.7 | 52.1 | 42.6 |
| HySCAN+ARS | 62.3 | 52.9 | 60.8 | 53.1 | 60.8 | 52.4 | 59.7 | 51.5 |


<table>
  <caption>
    <strong>Certified accuracy (%) of <code>HySCAN</code> and state-of-the-art defenses on <code>NIH-CXR</code>, <code>HAM10000</code>, and <code>CelebA</code>.</strong>
    All approaches are evaluated at three noise levels. Bold indicates the best results.
  </caption>
  <thead>
    <tr>
      <th rowspan="2">Approach</th>
      <th rowspan="2">σ</th>
      <th colspan="3">NIH-CXR (ℓ<sub>2</sub> radius r)</th>
      <th colspan="3">HAM10000 (ℓ<sub>2</sub> radius r)</th>
      <th colspan="3">CelebA (ℓ<sub>2</sub> radius r)</th>
    </tr>
    <tr>
      <th>0.0</th><th>0.50</th><th>1.0</th>
      <th>0.0</th><th>0.50</th><th>1.0</th>
      <th>0.0</th><th>0.50</th><th>1.0</th>
    </tr>
  </thead>
  <tbody>
    <!-- RS rows -->
    <tr><td rowspan="3">RS <sup>[1]</sup></td><td>0.25</td><td>77.4</td><td>43.5</td><td>15.7</td><td>94.6</td><td>53.2</td><td>10.5</td><td>92.8</td><td>45.7</td><td>0</td></tr>
    <tr><td>0.50</td><td>73.3</td><td>39.9</td><td>21.8</td><td>89.3</td><td>52.1</td><td>12.2</td><td>87.7</td><td>47.8</td><td>10.5</td></tr>
    <tr><td>1.0</td><td>66.4</td><td>42.9</td><td>22.8</td><td>84.7</td><td>54.3</td><td>21.2</td><td>81.4</td><td>51.6</td><td>18.8</td></tr>
    <!-- ARS rows -->
    <tr><td rowspan="3">ARS <sup>[2]</sup></td><td>0.25</td><td>79.1</td><td>58.4</td><td>32.5</td><td>96.7</td><td>57.4</td><td>31.3</td><td>95.2</td><td>53.3</td><td>27.4</td></tr>
    <tr><td>0.50</td><td>74.9</td><td>54.7</td><td>33.3</td><td>91.9</td><td>55.1</td><td>32.8</td><td>91.3</td><td>53.9</td><td>30.4</td></tr>
    <tr><td>1.0</td><td>69.9</td><td>52.9</td><td>34.1</td><td>86.9</td><td>57.4</td><td>34.6</td><td>85.3</td><td>59.2</td><td>31.6</td></tr>
    <!-- HySCAN rows -->
    <tr><td rowspan="3"><strong>HySCAN (Ours)</strong></td><td>0.25</td>
        <td><strong>81.2</strong></td><td><strong>63.1</strong></td><td><strong>39.4</strong></td>
        <td><strong>96.9</strong></td><td><strong>62.4</strong></td><td><strong>37.2</strong></td>
        <td><strong>96.5</strong></td><td><strong>59.7</strong></td><td><strong>34.9</strong></td></tr>
    <tr><td>0.50</td>
        <td><strong>76.1</strong></td><td><strong>59.6</strong></td><td><strong>42.3</strong></td>
        <td><strong>92.8</strong></td><td><strong>61.2</strong></td><td><strong>37.9</strong></td>
        <td><strong>92.5</strong></td><td><strong>60.7</strong></td><td><strong>36.1</strong></td></tr>
    <tr><td>1.0</td>
        <td><strong>71.4</strong></td><td><strong>61.1</strong></td><td><strong>42.9</strong></td>
        <td><strong>87.7</strong></td><td><strong>63.3</strong></td><td><strong>39.5</strong></td>
        <td><strong>87.4</strong></td><td><strong>63.9</strong></td><td><strong>38.4</strong></td></tr>
  </tbody>
</table>

<sub>[1] Cohen et al., 2019 – Randomized Smoothing (RS); 
[2] Lyu et al., 2024 – Adaptive RS (ARS).</sub>
