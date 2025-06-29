# Datasets for Trustworthy ML

A curated collection of datasets commonly used for research and education in trustworthy machine learning.

## Fairness Benchmarks

### Traditional ML Datasets

**[Adult Income Dataset](https://archive.ics.uci.edu/ml/datasets/Adult)**  
*UCI ML Repository* | 48K samples | Tabular  
```python
from aif360.datasets import AdultDataset
dataset = AdultDataset()
```
- **Task**: Income prediction (>$50K/year)
- **Protected attributes**: Race, gender, age
- **Use cases**: Group fairness, bias detection
- **Notable papers**: Most fairness papers use this dataset

**[COMPAS Recidivism](https://github.com/propublica/compas-analysis)**  
*ProPublica* | 7K samples | Tabular  
```python
from aif360.datasets import CompasDataset  
dataset = CompasDataset()
```
- **Task**: Recidivism risk prediction
- **Protected attributes**: Race, gender, age
- **Use cases**: Criminal justice fairness, algorithmic auditing
- **Real-world impact**: Used in actual court decisions

### Modern Fairness Benchmarks

**[Folktables](https://github.com/socialfoundations/folktables)**  
*Stanford* | Millions of samples | Census data  
```python
from folktables import ACSDataSource, ACSIncome
data_source = ACSDataSource(survey_year='2018', horizon='1-Year', survey='person')
```
- **Tasks**: Income, employment, health insurance, travel time
- **Features**: Realistic distribution shifts over time and geography  
- **Best for**: Large-scale fairness evaluation, intersectionality

**[CelebA](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)**  
*CUHK* | 200K images | Face attributes  
```python
import torchvision.datasets as datasets
dataset = datasets.CelebA(root='./data', download=True)
```
- **Task**: Multi-label face attribute prediction
- **Protected attributes**: Gender, apparent age, race (inferred)
- **Use cases**: Vision fairness, intersectional bias

## Robustness Benchmarks

### Adversarial Robustness

**[CIFAR-10/100](https://www.cs.toronto.edu/~kriz/cifar.html)**  
*University of Toronto* | 60K images | Object recognition  
```python
import torchvision.datasets as datasets
cifar10 = datasets.CIFAR10(root='./data', download=True)
```
- **Standard**: Most common robustness benchmark
- **Attacks**: FGSM, PGD, C&W, AutoAttack
- **Defenses**: Adversarial training, certified methods

**[ImageNet](https://www.image-net.org/)**  
*Stanford* | 14M images | Object recognition  
```python
from torchvision.datasets import ImageNet
dataset = ImageNet(root='./data', split='val')
```
- **Scale**: Large-scale robustness evaluation
- **Use cases**: Transfer learning robustness, real-world evaluation

### Distribution Shift

**[WILDS](https://wilds.stanford.edu/)**  
*Stanford* | Multiple domains | Distribution shift  
```python
from wilds import get_dataset
dataset = get_dataset(dataset="camelyon17", download=True)
```
- **Datasets**: Medical imaging, wildlife, satellite, text
- **Shifts**: Geographic, temporal, demographic
- **Evaluation**: Worst-group performance, average performance

**[ImageNet-C](https://github.com/hendrycks/robustness)**  
*UC Berkeley* | 15 corruption types | Corrupted images  
```python
# Download from authors' website
import numpy as np
corrupt_data = np.load('imagenet_c/gaussian_noise/5/') 
```
- **Corruptions**: Weather, blur, noise, digital artifacts
- **Severity**: 5 levels of corruption intensity
- **Use cases**: Natural robustness evaluation

## Privacy Benchmarks

### Federated Learning

**[LEAF](https://leaf.cmu.edu/)**  
*CMU* | Multiple tasks | Federated setting  
```python
# Use LEAF data loaders
from leaf.data_utils import read_data
clients, groups, data = read_data('femnist')
```
- **Datasets**: FEMNIST, CelebA, Reddit, Shakespeare
- **Properties**: Non-IID data distribution, realistic client heterogeneity
- **Use cases**: Federated learning algorithms, privacy evaluation

**[FLamby](https://flamby.github.io/)**  
*Inria* | Medical data | Cross-silo FL  
```python
from flamby.datasets.fed_heart_disease import FedHeartDisease
dataset = FedHeartDisease(center=0, train=True)
```
- **Focus**: Medical federated learning
- **Datasets**: Heart disease, skin cancer, drug discovery
- **Realistic**: Based on real medical collaborations

### Differential Privacy

**[Adult + DP Mechanisms](https://github.com/tensorflow/privacy)**  
*Google* | Various | DP training examples  
```python
from tensorflow_privacy.privacy.optimizers import dp_optimizer
optimizer = dp_optimizer.DPGradientDescentGaussianOptimizer(
    l2_norm_clip=1.0, noise_multiplier=1.1, learning_rate=0.01)
```
- **Benchmarks**: Standard datasets with DP training
- **Metrics**: Privacy budget vs. accuracy trade-offs

## Interpretability Datasets

### Feature Attribution

**[Boston Housing](https://www.cs.toronto.edu/~delve/data/boston/bostonDetail.html)**  
*UCI* | 506 samples | Regression  
```python
from sklearn.datasets import load_boston
X, y = load_boston(return_X_y=True)  # Note: deprecated due to ethical concerns
```
- **Use cases**: Feature importance, explanation evaluation
- **Note**: Consider alternatives due to ethical concerns

**[Wine Quality](https://archive.ics.uci.edu/ml/datasets/Wine+Quality)**  
*UCI* | 6K samples | Regression/Classification  
```python
import pandas as pd
data = pd.read_csv('winequality-red.csv', delimiter=';')
```
- **Features**: Chemical properties affecting wine quality
- **Use cases**: Feature attribution, counterfactual explanations

### Computer Vision

**[ImageNet + Attribution](https://github.com/PAIR-code/saliency)**  
*Google* | 14M images | Saliency evaluation  
```python
import saliency.core as saliency
gradient_saliency = saliency.GradientSaliency()
```
- **Methods**: GradCAM, Integrated Gradients, LIME
- **Evaluation**: Pointing game, deletion/insertion metrics

## Specialized Domains

### Natural Language Processing

**[BOLD](https://github.com/amazon-research/bold)**  
*Amazon* | Text generation | Bias evaluation  
```python
from bold import BoldDataset
dataset = BoldDataset()
```
- **Focus**: Bias in open-ended text generation
- **Attributes**: Gender, race, religion, political ideology
- **Metrics**: Sentiment, toxicity, regard

**[Winogender](https://github.com/rudinger/winogender-schemas)**  
*Johns Hopkins* | Coreference | Gender bias  
```python
import json
with open('data/winogender-schemas.txt') as f:
    templates = f.readlines()
```
- **Task**: Pronoun coreference resolution
- **Bias**: Gender stereotypes in occupations
- **Use cases**: NLP fairness evaluation

### Healthcare

**[MIMIC-III](https://mimic.mit.edu/)**  
*MIT* | 40K patients | Clinical records  
```python
# Requires credentialed access
import pandas as pd
admissions = pd.read_csv('ADMISSIONS.csv')
```
- **Access**: Requires training and approval
- **Use cases**: Healthcare fairness, privacy-preserving ML
- **Protected attributes**: Race, gender, insurance

### Finance

**[German Credit](https://archive.ics.uci.edu/ml/datasets/Statlog+(German+Credit+Data))**  
*UCI* | 1K samples | Credit risk  
```python
from aif360.datasets import GermanDataset
dataset = GermanDataset()
```
- **Task**: Credit risk assessment
- **Protected attributes**: Age, gender, foreign worker status
- **Use cases**: Financial fairness, regulatory compliance

## Dataset Usage Guidelines

### Fairness Analysis
1. **Identify protected attributes** in the dataset
2. **Define fairness metrics** appropriate for the task  
3. **Evaluate intersectional effects** across multiple attributes
4. **Consider historical bias** in data collection

### Robustness Testing
1. **Start with clean accuracy** as baseline
2. **Apply systematic attacks** with increasing strength
3. **Test multiple threat models** (white-box, black-box)
4. **Evaluate on distribution shifts** relevant to deployment

### Privacy Evaluation  
1. **Implement membership inference attacks** as baseline
2. **Measure privacy-utility trade-offs** across ε values
3. **Test reconstruction attacks** where applicable
4. **Validate privacy guarantees** with formal analysis

## Ethical Considerations

### Data Usage
- **Consent**: Ensure appropriate consent for research use
- **Bias**: Acknowledge limitations and potential biases
- **Privacy**: Follow data protection regulations (GDPR, etc.)
- **Attribution**: Cite original data sources appropriately

### Sensitive Attributes
- **Protected characteristics**: Handle race, gender, etc. with care
- **Intersectionality**: Consider multiple overlapping identities
- **Historical context**: Understand societal biases in data
- **Representation**: Ensure diverse and inclusive datasets

---

!!! warning "Dataset Deprecations"
    Some datasets (e.g., Boston Housing) have been deprecated due to ethical concerns. Always check for recommended alternatives and consider the ethical implications of your dataset choices.

*Last updated: December 2024*