# 如何使用预测建模进行数据驱动的预测

> 原文：<https://www.dominodatalab.com/blog/introduction-to-predictive-modeling>

当你听到机器学习(ML)或人工智能(AI)这样的词时，首先想到的事情之一是正确预测未来的发生或根据过去的事件回答关于现在的困难问题。从本质上讲，这就是预测建模的意义所在。

## 什么是预测建模？

预测建模是一种机器学习技术，它基于历史和当前数据预测或预测可能的未来结果。[](https://www.brunswickgroup.com/domino-data-lab-nick-elprin-i8822/)预测模型可以用来预测任何事情，包括贷款风险和天气预报，以及你下一个最喜欢的电视节目。通常，预测会描述一些情况，比如一笔 [信用卡交易是否是欺诈性的](https://blog.dominodatalab.com/credit-card-fraud-detection-using-xgboost-smote-and-threshold-moving) 或者一个病人是否有心脏病。

## 预测建模是如何工作的？

在开发和部署机器学习解决方案时，模型驱动的组织遵循 [四阶段数据科学生命周期](https://blog.dominodatalab.com/how-enterprise-mlops-works-throughout-the-data-science-lifecycle) :管理、开发、部署和监控。

### 经营

预测建模通常从一个需要解决的问题或问题陈述开始。这些问题千差万别，而且不乏此类问题，例如:

*   我们应该订购多少存货？
*   我们应该什么时候投资？
*   我们需要多少张病床？

一旦你明确了你的问题，你就需要收集一个与这个问题相关的数据集。例如，如果您正在建立销售预测模型，您需要销售数据。该项目应优先于其他项目，以将数据科学资源集中在最有价值的地方。

### 发展

在开发阶段，您首先要探索哪些预测算法最适合用您现有的数据来回答您的问题。

与此同时，您需要清理和分析数据，以确保它可供您的算法使用。清理数据包括删除重复数据、无关变量以及确保数据标准化。例如，来自不同来源的数据通常会有不同的格式，常见的例子有州缩写或产品 SKU。您还需要检查空值、异常值，并确保占位符出现在需要的地方。

将数据分为训练集和测试或验证集，可以让您在一组数据上训练模型，然后在另一组数据上测试它，从而避免削弱或过度拟合。在将数据分成两组后对其进行预处理有助于避免数据泄漏。

在相同的训练数据集上测试每个候选模型。然后使用测试集再次运行每个模型。有了这些测试的结果，您就可以评估模型结果，以确定哪个模型的性能最好。这一步总是高度迭代的，因此在选择最终模型之前，您可能会多次循环查找数据、准备数据、构建模型和测试模型。

### 部署

一旦您有了一个为您提供满意结果的模型，您就可以进入部署阶段，将模型迁移到一个真实的环境中。这可能涉及到构建应用程序、使用 API 或在数据库中部署模型。在这一点上，最终用户被介绍到模型中，并被训练以任何形式使用其结果。

### 班长

模型部署后，需要对其进行[监控](https://www.dominodatalab.com/blog/model-monitoring-best-practices-maintaining-data-science-at-scale)以确保其在预期参数内继续运行。如果模型开始漂移，可能需要将其移除并重新部署。同样重要的是监控模型所输入的数据。如果数据的类型或格式与训练数据不同，则模型可能会开始生成意外的结果。

一旦模型被认为运行不正常，迅速采取措施补救这种情况并重新部署模型是至关重要的。

![Data scientist looking at a predictive model](img/6bb07e66b66504a1d83788ee646500ae.png)

### 不准确或不可接受的预测

无论使用何种技术，模型的预测或预报能力都受到它必须处理的数据的限制。例如，这经常是预测流行病的问题。当一种新病毒出现时，或现有病毒的变种出现时，预测模型会受到现有数据的限制。如果关于类似病毒或变种的现有数据不能反映新毒株的实际情况，那么对医院床位需求的预测，或者对关闭的结果的预测，就不会准确。

在其他情况下，模型可能是准确的，但由于模型偏差，提供的结果会产生比它们解决的问题更多的问题。美国刑事司法系统使用的预测模型在预测社区犯罪热点或未来违反假释时，经常向执法部门提供带有种族偏见的结果。即使当种族作为一个数据变量被删除，其他相关变量如地理或收入也可能无意中把种族预测带回到结果中。

## 预测模型的重要性

成千上万的组织正在使用 Domino 的企业 MLOps 平台来改进他们的预测建模方法，在[](https://www.dominodatalab.com/customers/fortune-500-insurer)欺诈检测方面取得了进步，确定了早期癌症 的新 [预测因子，甚至帮助农民](https://analytics-solution.pharmatechoutlook.com/vendor/domino-data-lab-imbuing-innovation-in-modeldriven-businesses-cid-324-mid-38.html) [更高效地种植作物](https://www.dominodatalab.com/customers/bayer) 并提高产量。

想象一下，例如，以 99.9%的准确率知道你的投资将会盈利的可能性，或者如果你的汽车发动机今天不维修，明天就会出故障。成功的数据科学项目需要在准确性、可靠性、成本和盈利能力之间找到恰当的平衡点。能够在规模上平衡这些变量是一个盈利的数据模型组织的区别。

### 预测建模用例

当预测建模做得正确时，不可否认它会带来巨大的回报。成功的一个关键因素是在 MLOps 平台上工作，该平台可为您的数据科学团队提供所需的工具和资源，以便在协作和记录完善的环境中出色完成工作。

#### Domino 数据实验室的预测建模

Forrester 的一项新研究显示，通过使用 Domino 的数据科学平台，公司可以实现 542%的投资回报率[](https://www.dominodatalab.com/domino-business-impact-forrester-tei-report/)。2021 年 2 月，洛克希德·马丁公司宣布，通过使用 Domino 数据科学平台扩展其 AI/ML 解决方案，该公司已经实现了超过[](https://www.dominodatalab.com/news/domino-data-lab-helps-lockheed-martin-advance-data-science-and-analytics-3)2000 万美元的年价值。

最重要的是，要记住预测建模是一门科学。成功的、模型驱动的组织就是这样对待它的，而那些不这样做的组织只会在碰运气的基础上取得成功。为了找出史蒂夫·沃兹尼亚克说“多米诺数据实验室机器学习操作正在改变世界”的原因， [观看一个演示](https://www.dominodatalab.com/demo/) 它的行动。你也可以用一个 [免费试用](https://www.dominodatalab.com/trial/) 开始探索它的特性。

David Weedmark 是一位出版作家，曾担任过项目经理、软件开发人员和网络安全顾问。