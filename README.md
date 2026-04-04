# 🫘 Bean Classification Deep Learning Project

![Python](https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.15-orange?style=for-the-badge&logo=tensorflow)
![Status](https://img.shields.io/badge/Status-Production%20Ready-green?style=for-the-badge)

## 🎯 Overview
هذا المشروع يهدف إلى بناء وتدريب نموذج ذكاء اصطناعي (Deep Learning) قادر على تصنيف **7 أنواع مختلفة من البقوليات** بدقة عالية تصل إلى **94%**. تم التركيز في هذا المشروع على دورة حياة نموذج الـ Machine Learning بالكامل، من معالجة البيانات وصولاً إلى الـ Deployment.

## 🚀 Key Features
* **Data Engineering**: استخدام تقنيات متقدمة لمعالجة البيانات والـ Scaling.
* **Automated Tuning**: استخدام `KerasTuner` للبحث عن أفضل معمارية للنموذج.
* **Professional Evaluation**: تقييم شامل باستخدام `Confusion Matrix` و `Classification Report`.
* **Deployment Ready**: توفير الموديل مع الـ Scaler للاستخدام في تطبيقات حقيقية.

## 🏗️ Project Architecture
[attachment_0](attachment)

## 📈 Results
حقق النموذج أداءً متميزاً في تصنيف الفئات السبعة:
* **Overall Accuracy**: 94%.
* **Model Robustness**: قدرة عالية على التعميم بفضل استخدام `Dropout` و `L2 Regularization`.

## 📊 Training Results & Evaluation

### 1. Model Training History (Loss & Accuracy)
The following graphs illustrate the model's performance during the training and validation phases over epochs.

![Training Accuracy](<   <img width="719" height="585" alt="graph_accuracy" src="https://github.com/user-attachments/assets/bc8de5d8-d585-47ea-984e-c1665bc24f3c" />
 >)

تحليل منحنى دقة النموذج (Model Accuracy Analysis)

​يعرض الرسم البياني أداء نموذج تعلم عميق خلال مراحل التدريب والاختبار على مدار 50 حقبة (Epoch). يوضح المنحنى استقراراً ملحوظاً وتقارباً بين دقة التدريب (Train) ودقة الاختبار (Test)، حيث وصلت الدقة إلى ما يقارب 90%. يشير هذا النمط إلى كفاءة النموذج وقدرته العالية على التعميم (Generalization) دون الوقوع في مشكلة الإفراط في التخصيص (Overfitting)

​English

​Title: Model Accuracy Performance Curve
​This graph illustrates the performance of a deep learning model during the training and validation phases over 50 epochs. The curves show a steady increase in accuracy, eventually plateauing at approximately 90%. The close proximity between the training and testing lines indicates strong model generalization and suggests that the model is well-tuned with minimal overfitting.


![Training Loss](<<img width="730" height="581" alt="graph_Loss" src="https://github.com/user-attachments/assets/8a05cd83-00e4-4da5-b0ab-91a0349bd076" />>)

تحليل منحنى خسارة النموذج (Model Loss Analysis)

​يوضح هذا الرسم البياني انخفاض معدل الخسارة (Loss) للنموذج خلال مراحل التدريب والتحقق (Validation) على مدار 50 حقبة. نلاحظ هبوطاً حاداً وسريعاً في البداية، يتبعه استقرار تدريجي عند مستويات منخفضة تقترب من 0.2. التوازي المستمر بين منحنى التدريب والتحقق يشير إلى أن النموذج يتعلم بشكل صحيح ومستقر، مما يؤكد جودة عملية التحسين (Optimization) التي تمت أثناء التدريب

​English

​Title: Model Loss Performance Curve
​This graph displays the reduction in loss during the training and validation phases over 50 epochs. The curves show a sharp initial decline, followed by a steady convergence towards a minimum value of approximately 0.2. The consistent alignment between the training and validation loss indicates a stable learning process and effective optimization, confirming that the model is avoiding divergence or overfitting issues.

### 2. Confusion Matrix
This matrix helps in understanding the model's performance across different classes and identifying where it might be making errors.

![Confusion Matrix](< <img width="1023" height="638" alt="Confusion_Matrix" src="https://github.com/user-attachments/assets/a1addeca-5584-46e6-8c1e-5489a6c0b74a" />>)

تحليل مصفوفة الارتباك (Confusion Matrix Analysis)

​توضح هذه المصفوفة تفاصيل أداء النموذج في تصنيف الفئات المختلفة. يشير القطر الرئيسي المظلل باللون الأزرق الداكن إلى عدد التوقعات الصحيحة لكل فئة، حيث نلاحظ دقة عالية جداً في الفئة رقم 3 (669 توقعاً صحيحاً) والفئة رقم 5 (387 توقعاً صحيحاً). تشير القيم المنخفضة خارج القطر الرئيسي إلى وجود تداخل طفيف جداً بين بعض الفئات، مما يؤكد أن النموذج يمتلك قدرة تمييزية (Discriminative Power) قوية بين الطبقات المختلفة.

​English

​Title: Confusion Matrix Evaluation
​This matrix provides a detailed breakdown of the model's classification performance across multiple classes. The dark blue diagonal represents the true positive predictions for each class, showing exceptional accuracy particularly in Class 3 (669 correct hits) and Class 5 (387 correct hits). The minimal off-diagonal values indicate very low misclassification rates, confirming the model's strong discriminative power and high precision in distinguishing between the target categories.

### 3. Classification Report 
Detailed metrics including Precision, Recall, and F1-score for each class.

![Classification Report](< <img width="553" height="326" alt="Classification_Report" src="https://github.com/user-attachments/assets/4a9978de-35ce-4756-968f-ade09e228c2d" />>)

تقرير تقييم أداء النموذج (Detailed Classification Report)

​يوضح هذا التقرير مقاييس الأداء التفصيلية لكل فئة من فئات البيانات، حيث حقق النموذج دقة إجمالية (Accuracy) تصل إلى 93%. يتضح من خلال قيم الـ F1-score والـ Precision أن النموذج يحقق توازناً مثالياً في التصنيف، خاصة في الفئة رقم 1 التي سجلت علامة كاملة تقريباً. استقرار متوسطات الماكرو (Macro Avg) والوزن (Weighted Avg) عند 93% و 94% يؤكد أن النموذج لا يعاني من انحياز لفئة معينة ويؤدي بكفاءة عالية على كامل مجموعة البيانات.

​English

​Title: Classification Performance Report
​This report summarizes the key evaluation metrics for each class, with the model achieving an overall Accuracy of 93%. The high Precision, Recall, and F1-score across all categories, particularly Class 1 which scored a perfect 1.00, demonstrate a highly robust model. The Macro and Weighted averages (stabilizing at 93-94%) confirm that the model is well-balanced and performs consistently across all classes without being biased toward the majority labels.

## 🛠️ Tech Stack
* **Language**: Python
* **Frameworks**: TensorFlow, Keras, Scikit-Learn
* **Optimization**: KerasTuner
* **Visualization**: Seaborn, Matplotlib

## 👤 Author
**[MOHAMED BELAL]** *Deep Learning & Data Engineering Enthusiast*

MY PHONE [01018689118]
