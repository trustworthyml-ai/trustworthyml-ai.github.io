# Tools & Frameworks

A comprehensive collection of open-source tools, libraries, and frameworks for implementing trustworthy machine learning systems.

## Fairness & Bias Mitigation

### Comprehensive Toolkits

**[AI Fairness 360 (AIF360)](https://aif360.mybluemix.net/)**  
*IBM Research* | Python, R | ⭐⭐⭐⭐⭐  
```bash
pip install aif360
```
- **Features**: 70+ fairness metrics, 10+ bias mitigation algorithms
- **Best for**: Research, comprehensive bias analysis, enterprise applications
- **Highlights**: Web interface, extensive documentation, industry-tested
- **Example**: Credit scoring, hiring decisions, criminal justice

**[Fairlearn](https://fairlearn.org/)**  
*Microsoft* | Python | ⭐⭐⭐⭐  
```bash
pip install fairlearn
```
- **Features**: Scikit-learn integration, dashboard visualization, constraint-based optimization
- **Best for**: Quick prototyping, ML practitioners familiar with sklearn
- **Highlights**: User-friendly API, interactive dashboards, Azure ML integration

### Specialized Libraries

**[Themis](https://github.com/LASER-UMASS/Themis)**  
*UMass Amherst* | Python | ⭐⭐⭐  
```bash
pip install themis-ml
```
- **Focus**: Fairness testing and debugging
- **Features**: Automated bias discovery, causal fairness analysis
- **Best for**: Testing existing models for hidden biases

**[FairML](https://github.com/adebayoj/fairml)**  
*Academic* | Python | ⭐⭐⭐  
```bash
pip install fairml
```
- **Focus**: Auditing black-box models
- **Features**: Input influence ranking, bias detection without model access
- **Best for**: Third-party model auditing

## Robustness & Adversarial Defense

### Attack Libraries

**[Adversarial Robustness Toolbox (ART)](https://adversarial-robustness-toolbox.org/)**  
*IBM Research* | Python | ⭐⭐⭐⭐⭐  
```bash
pip install adversarial-robustness-toolbox
```
- **Features**: 20+ attacks, 15+ defenses, multiple ML frameworks
- **Frameworks**: TensorFlow, PyTorch, scikit-learn, XGBoost
- **Best for**: Comprehensive adversarial ML research and testing

**[Foolbox](https://foolbox.readthedocs.io/)**  
*University of Tübingen* | Python | ⭐⭐⭐⭐  
```bash
pip install foolbox
```
- **Features**: 30+ gradient-based and black-box attacks
- **Frameworks**: PyTorch, TensorFlow, JAX, NumPy
- **Best for**: Quick adversarial example generation, benchmarking

**[CleverHans](https://github.com/cleverhans-lab/cleverhans)**  
*Google Brain* | Python | ⭐⭐⭐  
```bash
pip install cleverhans
```
- **Features**: Classic attacks (FGSM, PGD, C&W), TensorFlow focus
- **Best for**: Educational purposes, reproducing classic papers

### Defense Frameworks

**[CROWN](https://github.com/huanzhang12/CROWN-IBP)**  
*UCLA* | Python | ⭐⭐⭐⭐  
```bash
git clone https://github.com/huanzhang12/CROWN-IBP
```
- **Focus**: Certified robustness via interval bound propagation
- **Features**: Formal verification, scalable certified training
- **Best for**: Safety-critical applications requiring guarantees

**[Auto-Attack](https://github.com/fra31/auto-attack)**  
*EPFL* | Python | ⭐⭐⭐⭐  
```bash
pip install autoattack
```
- **Focus**: Robust evaluation standard
- **Features**: Ensemble of complementary attacks, parameter-free
- **Best for**: Standardized robustness evaluation

## Interpretability & Explainability

### Model-Agnostic Tools

**[SHAP](https://shap.readthedocs.io/)**  
*Microsoft Research* | Python | ⭐⭐⭐⭐⭐  
```bash
pip install shap
```
- **Theory**: Shapley values from cooperative game theory
- **Features**: Global/local explanations, 15+ explainer types
- **Visualization**: Interactive plots, force plots, dependence plots
- **Best for**: Production explanations, business stakeholders

**[LIME](https://github.com/marcotcr/lime)**  
*University of Washington* | Python | ⭐⭐⭐⭐  
```bash
pip install lime
```
- **Theory**: Local linear approximation
- **Features**: Text, image, tabular data support
- **Best for**: Quick local explanations, diverse data types

### Deep Learning Specific

**[Captum](https://captum.ai/)**  
*PyTorch Team* | Python | ⭐⭐⭐⭐⭐  
```bash
pip install captum
```
- **Framework**: Native PyTorch integration
- **Features**: 15+ attribution algorithms, neuron/layer analysis
- **Visualization**: Built-in visualization utilities
- **Best for**: Deep learning research, PyTorch users

**[Alibi](https://docs.seldon.io/projects/alibi/)**  
*Seldon* | Python | ⭐⭐⭐⭐  
```bash
pip install alibi
```
- **Features**: Counterfactual explanations, anchor explanations
- **Focus**: Production-ready explanations for ML deployment
- **Best for**: Model serving, real-time explanations

**[InterpretML](https://interpret.ml/)**  
*Microsoft Research* | Python | ⭐⭐⭐⭐  
```bash
pip install interpret
```
- **Features**: Glass-box models (EBM), model-agnostic explanations
- **Visualization**: Unified dashboard for multiple explanation types
- **Best for**: Regulated industries, healthcare, finance

## Privacy-Preserving ML

### Differential Privacy

**[Opacus](https://opacus.ai/)**  
*PyTorch Team* | Python | ⭐⭐⭐⭐⭐  
```bash
pip install opacus
```
- **Framework**: PyTorch-native differential privacy
- **Features**: DP-SGD, privacy accounting, gradient clipping
- **Best for**: Deep learning with formal privacy guarantees

**[TensorFlow Privacy](https://github.com/tensorflow/privacy)**  
*Google* | Python | ⭐⭐⭐⭐  
```bash
pip install tensorflow-privacy
```
- **Framework**: TensorFlow integration
- **Features**: DP optimizers, privacy analysis, membership inference
- **Best for**: Large-scale DP training, Google Cloud integration

**[Diffprivlib](https://diffprivlib.readthedocs.io/)**  
*IBM Research* | Python | ⭐⭐⭐⭐  
```bash
pip install diffprivlib
```
- **Framework**: Scikit-learn compatible DP algorithms
- **Features**: DP versions of common ML algorithms
- **Best for**: Traditional ML with differential privacy

### Federated Learning

**[PySyft](https://github.com/OpenMined/PySyft)**  
*OpenMined* | Python | ⭐⭐⭐⭐  
```bash
pip install syft
```
- **Features**: Federated learning, secure multi-party computation
- **Frameworks**: PyTorch, TensorFlow support
- **Best for**: Research, privacy-preserving collaborations

**[Flower (flwr)](https://flower.dev/)**  
*Flower Labs* | Python | ⭐⭐⭐⭐⭐  
```bash
pip install flwr
```
- **Features**: Framework-agnostic federated learning
- **Deployment**: Easy client-server architecture
- **Best for**: Production federated learning, cross-platform deployment

**[FedML](https://fedml.ai/)**  
*FedML Inc* | Python | ⭐⭐⭐⭐  
```bash
pip install fedml
```
- **Features**: MLOps for federated learning, mobile deployment
- **Platform**: Cloud platform + open source library
- **Best for**: End-to-end federated ML solutions

## Evaluation & Benchmarking

### Robustness Benchmarks

**[RobustBench](https://robustbench.github.io/)**  
*Community* | Python | ⭐⭐⭐⭐⭐  
```bash
pip install robustbench
```
- **Features**: Standardized robustness evaluation, model zoo
- **Datasets**: CIFAR-10/100, ImageNet, common corruptions
- **Best for**: Comparing robustness methods, reproducible evaluation

### Fairness Benchmarks

**[Folktables](https://github.com/socialfoundations/folktables)**  
*Stanford* | Python | ⭐⭐⭐⭐  
```bash
pip install folktables
```
- **Features**: Real-world fairness benchmarks from US Census data
- **Tasks**: Income prediction, employment, health insurance
- **Best for**: Realistic fairness evaluation, policy research

## Development & Deployment

### MLOps for Trustworthy ML

**[Evidently](https://evidentlyai.com/)**  
*Evidently AI* | Python | ⭐⭐⭐⭐  
```bash
pip install evidently
```
- **Features**: ML monitoring, drift detection, bias monitoring
- **Deployment**: Dashboard, reports, real-time monitoring
- **Best for**: Production ML monitoring, continuous auditing

**[Great Expectations](https://greatexpectations.io/)**  
*Superconductive* | Python | ⭐⭐⭐⭐  
```bash
pip install great-expectations
```
- **Features**: Data validation, pipeline testing, documentation
- **Integration**: Airflow, dbt, cloud platforms
- **Best for**: Data quality assurance, ML pipeline validation

### Model Cards & Documentation

**[Model Card Toolkit](https://github.com/tensorflow/model-card-toolkit)**  
*Google* | Python | ⭐⭐⭐  
```bash
pip install model-card-toolkit
```
- **Features**: Automated model card generation, templates
- **Integration**: TensorFlow Model Analysis integration
- **Best for**: Model documentation, regulatory compliance

## Quick Start Guides

### Fairness Analysis Workflow
```python
# Using AIF360 for comprehensive bias analysis
from aif360.datasets import AdultDataset
from aif360.metrics import BinaryLabelDatasetMetric
from aif360.algorithms.preprocessing import Reweighing

# Load data and compute bias metrics
dataset = AdultDataset()
metric = BinaryLabelDatasetMetric(dataset)
print(f"Disparate Impact: {metric.disparate_impact()}")

# Apply bias mitigation
rw = Reweighing(unprivileged_groups=[{'sex': 0}],
                privileged_groups=[{'sex': 1}])
dataset_transf = rw.fit_transform(dataset)
```

### Adversarial Robustness Testing
```python
# Using ART for adversarial evaluation
from art.attacks.evasion import FastGradientMethod
from art.estimators.classification import KerasClassifier

# Wrap your model
classifier = KerasClassifier(model=model)

# Generate adversarial examples
attack = FastGradientMethod(estimator=classifier, eps=0.1)
x_test_adv = attack.generate(x=x_test)

# Evaluate robustness
accuracy_clean = classifier.predict(x_test).argmax(axis=1) == y_test
accuracy_adv = classifier.predict(x_test_adv).argmax(axis=1) == y_test
print(f"Clean accuracy: {accuracy_clean.mean():.2f}")
print(f"Adversarial accuracy: {accuracy_adv.mean():.2f}")
```

### Privacy-Preserving Training
```python
# Using Opacus for differential privacy
from opacus import PrivacyEngine

# Attach privacy engine to optimizer
privacy_engine = PrivacyEngine()
model, optimizer, data_loader = privacy_engine.make_private(
    module=model,
    optimizer=optimizer,
    data_loader=data_loader,
    noise_multiplier=1.0,
    max_grad_norm=1.0,
)

# Train with privacy guarantees
for epoch in range(epochs):
    for batch in data_loader:
        # Standard PyTorch training loop
        optimizer.zero_grad()
        loss = criterion(model(batch[0]), batch[1])
        loss.backward()
        optimizer.step()
    
    # Check privacy budget
    epsilon = privacy_engine.get_epsilon(delta=1e-5)
    print(f"Epoch {epoch}, ε = {epsilon:.2f}")
```

---

!!! tip "Tool Selection Guide"
    - **Research**: Start with comprehensive toolkits (AIF360, ART, SHAP)
    - **Production**: Focus on framework-specific tools (Fairlearn for sklearn, Captum for PyTorch)
    - **Evaluation**: Use standardized benchmarks (RobustBench, Folktables)
    - **Deployment**: Implement monitoring (Evidently, Great Expectations)

*Last updated: December 2024*