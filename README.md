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

<!-- Empirical robustness table (ℓ∞, APGD-20 & AA-20) -->
<table>
  <caption>
    <strong>Empirical robustness (accuracy&nbsp;%) against ℓ<sub>∞</sub> adversarial attacks</strong>
    &nbsp;(APGD-20 and AA-20) on <code>NCT-CRC-HE-100K</code> (left) and <code>NIH-CXR</code> (right) at
    ε ∈ {8/255, 16/255}. Values in parentheses are standard deviations.
  </caption>

  <!-- Header rows -->
  <thead>
    <tr>
      <th rowspan="3">Method</th>
      <th colspan="5">NCT-CRC-HE-100K</th>
      <th colspan="5">NIH-CXR</th>
    </tr>
    <tr>
      <th rowspan="2">Clean</th>
      <th colspan="2">APGD-20</th>
      <th colspan="2">AA-20</th>
      <th rowspan="2">Clean</th>
      <th colspan="2">APGD-20</th>
      <th colspan="2">AA-20</th>
    </tr>
    <tr>
      <th>8/255</th><th>16/255</th><th>8/255</th><th>16/255</th>
      <th>8/255</th><th>16/255</th><th>8/255</th><th>16/255</th>
    </tr>
  </thead>

  <!-- Body -->
  <tbody>
    <tr style="background:#f7f7f7">
      <td><em>DRS</em></td>
      <td>85.9 (2.25)</td><td>75.1 (2.61)</td><td>65.2 (3.82)</td><td>73.5 (3.21)</td><td>63.7 (3.94)</td>
      <td>83.9 (2.33)</td><td>73.1 (2.41)</td><td>62.9 (3.23)</td><td>71.6 (3.12)</td><td>61.9 (3.81)</td>
    </tr>
    <tr>
      <td><em>ARS</em></td>
      <td>86.8 (2.14)</td><td>75.9 (2.71)</td><td>66.1 (3.52)</td><td>74.6 (3.11)</td><td>64.5 (3.73)</td>
      <td>84.8 (2.22)</td><td>75.1 (3.01)</td><td>64.7 (3.28)</td><td>72.8 (3.11)</td><td>62.8 (3.72)</td>
    </tr>
    <tr style="background:#f7f7f7">
      <td><em>AT</em></td>
      <td>92.2 (1.82)</td><td>77.8 (2.51)</td><td>68.7 (3.12)</td><td>76.3 (2.83)</td><td>66.2 (3.61)</td>
      <td>89.1 (1.91)</td><td>74.7 (2.52)</td><td>66.9 (3.41)</td><td>74.2 (2.93)</td><td>64.1 (3.70)</td>
    </tr>
    <tr>
      <td><em>DCS</em></td>
      <td>90.3 (1.93)</td><td>84.5 (2.72)</td><td>73.0 (3.25)</td><td>83.3 (2.74)</td><td>71.6 (3.46)</td>
      <td>87.2 (2.05)</td><td>82.4 (2.41)</td><td>71.7 (3.21)</td><td>81.7 (2.72)</td><td>69.6 (3.45)</td>
    </tr>
    <tr style="background:#f7f7f7">
      <td><em>CTRW</em></td>
      <td>90.4 (1.62)</td><td>87.6 (2.29)</td><td>76.7 (3.12)</td><td>86.7 (2.44)</td><td>75.2 (3.22)</td>
      <td>88.4 (1.73)</td><td>85.1 (2.23)</td><td>73.1 (3.22)</td><td>84.5 (2.48)</td><td>72.6 (3.41)</td>
    </tr>
    <tr>
      <td><em>RPF</em></td>
      <td>91.1 (1.71)</td><td>86.1 (2.33)</td><td>73.9 (3.33)</td><td>84.2 (2.62)</td><td>72.4 (3.41)</td>
      <td>88.4 (1.82)</td><td>83.7 (2.49)</td><td>71.9 (3.29)</td><td>82.5 (2.71)</td><td>70.8 (3.52)</td>
    </tr>
    <tr>
      <td><em>HyCAS</em></td>
      <td>91.3 (2.63)</td><td>90.4 (2.82)</td><td>79.3 (3.52)</td><td>88.2 (2.63)</td><td>76.7 (3.34)</td>
      <td>89.5 (1.64)</td><td>88.6 (2.33)</td><td>77.3 (3.14)</td><td>86.9 (2.42)</td><td>74.4 (3.33)</td>
    </tr>
    <tr style="background:#f7f7f7;font-weight:bold">
      <td>HySCAN (Ours)</td>
      <td>91.5 (2.25)</td><td>90.7 (1.69)</td><td>80.2 (2.61)</td><td>89.5 (1.24)</td><td>77.3 (2.98)</td>
      <td>90.1 (0.87)</td><td>88.9 (1.75)</td><td>78.1 (2.82)</td><td>87.3 (1.98)</td><td>75.1 (2.59)</td>
    </tr>
  </tbody>
</table>






<!-- Empirical robustness table: NCT-CRC-HE-100K (left) and NIH-CXR (right) -->
<table>
  <caption>
    <strong>Empirical robustness (accuracy&nbsp;%) against ℓ<sub>∞</sub> attacks (APGD-20 and AA-20)</strong><br>
    Datasets: <code>NCT-CRC-HE-100K</code> and <code>NIH-CXR</code>; perturbation strengths ε ∈ {8/255, 16/255}.<br>
    Values in parentheses are standard deviations.
  </caption>

  <!-- Header rows -->
  <thead>
    <tr>
      <th rowspan="3">Method</th>
      <th colspan="5">NCT-CRC-HE-100K</th>
      <th colspan="5">NIH-CXR</th>
    </tr>
    <tr>
      <th rowspan="2">Clean</th>
      <th colspan="2">APGD-20</th>
      <th colspan="2">AA-20</th>
      <th rowspan="2">Clean</th>
      <th colspan="2">APGD-20</th>
      <th colspan="2">AA-20</th>
    </tr>
    <tr>
      <th>8/255</th><th>16/255</th>
      <th>8/255</th><th>16/255</th>
      <th>8/255</th><th>16/255</th>
      <th>8/255</th><th>16/255</th>
    </tr>
  </thead>

  <!-- Body rows -->
  <tbody>
    <!-- DRS -->
    <tr>
      <td><em>DRS</em><sup>[1]</sup></td>
      <td>85.9 (2.25)</td><td>75.1 (2.61)</td><td>65.2 (3.82)</td><td>73.5 (3.21)</td><td>63.7 (3.94)</td>
      <td>83.9 (2.33)</td><td>73.1 (2.41)</td><td>62.9 (3.23)</td><td>71.6 (3.12)</td><td>61.9 (3.81)</td>
    </tr>
    <!-- ARS -->
    <tr>
      <td><em>ARS</em><sup>[2]</sup></td>
      <td>86.8 (2.14)</td><td>75.9 (2.71)</td><td>66.1 (3.52)</td><td>74.6 (3.11)</td><td>64.5 (3.73)</td>
      <td>84.8 (2.22)</td><td>75.1 (3.01)</td><td>64.7 (3.28)</td><td>72.8 (3.11)</td><td>62.8 (3.72)</td>
    </tr>
    <!-- AT -->
    <tr>
      <td><em>AT</em><sup>[3]</sup></td>
      <td>92.2 (1.82)</td><td>77.8 (2.51)</td><td>68.7 (3.12)</td><td>76.3 (2.83)</td><td>66.2 (3.61)</td>
      <td>89.1 (1.91)</td><td>74.7 (2.52)</td><td>66.9 (3.41)</td><td>74.2 (2.93)</td><td>64.1 (3.70)</td>
    </tr>
    <!-- DCS -->
    <tr>
      <td><em>DCS</em><sup>[4]</sup></td>
      <td>90.3 (1.93)</td><td>84.5 (2.72)</td><td>73.0 (3.25)</td><td>83.3 (2.74)</td><td>71.6 (3.46)</td>
      <td>87.2 (2.05)</td><td>82.4 (2.41)</td><td>71.7 (3.21)</td><td>81.7 (2.72)</td><td>69.6 (3.45)</td>
    </tr>
    <!-- CTRW -->
    <tr>
      <td><em>CTRW</em><sup>[5]</sup></td>
      <td>90.4 (1.62)</td><td>87.6 (2.29)</td><td>76.7 (3.12)</td><td>86.7 (2.44)</td><td>75.2 (3.22)</td>
      <td>88.4 (1.73)</td><td>85.1 (2.23)</td><td>73.1 (3.22)</td><td>84.5 (2.48)</td><td>72.6 (3.41)</td>
    </tr>
    <!-- RPF -->
    <tr>
      <td><em>RPF</em><sup>[6]</sup></td>
      <td>91.1 (1.71)</td><td>86.1 (2.33)</td><td>73.9 (3.33)</td><td>84.2 (2.62)</td><td>72.4 (3.41)</td>
      <td>88.4 (1.82)</td><td>83.7 (2.49)</td><td>71.9 (3.29)</td><td>82.5 (2.71)</td><td>70.8 (3.52)</td>
    </tr>
    <!-- HyCAS -->
    <tr>
      <td><em>HyCAS</em><sup>[6]</sup></td>
      <td>91.3 (2.63)</td><td>90.4 (2.82)</td><td>79.3 (3.52)</td><td>88.2 (2.63)</td><td>76.7 (3.34)</td>
      <td>89.5 (1.64)</td><td>88.6 (2.33)</td><td>77.3 (3.14)</td><td>86.9 (2.42)</td><td>74.4 (3.33)</td>
    </tr>
    <!-- HySCAN -->
    <tr>
      <td><strong>HySCAN&nbsp;(Ours)</strong></td>
      <td><strong>91.5 (2.25)</strong></td><td><strong>90.7 (1.69)</strong></td><td><strong>80.2 (2.61)</strong></td><td><strong>89.5 (1.24)</strong></td><td><strong>77.3 (2.98)</strong></td>
      <td><strong>90.1 (0.87)</strong></td><td><strong>88.9 (1.75)</strong></td><td><strong>78.1 (2.82)</strong></td><td><strong>87.3 (1.98)</strong></td><td><strong>75.1 (2.59)</strong></td>
    </tr>
  </tbody>
</table>

<sub>
[1] Xia et al., 2024 · DRS   
[2] Lyu et al., 2024 · ARS   
[3] Madry et al., 2018 · AT   
[4] Ma et al., 2023 · DCS   
[5] Ma et al., 2023 · CTRW   
[6] Dong et al., 2023 · RPF / HyCAS
</sub>

