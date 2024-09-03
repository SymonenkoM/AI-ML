Summary
Purpose: The code aims to build a simple linear regression model to predict an employee's salary based on their years of experience.
Data Handling: It involves loading data, splitting it into training and testing sets, training a model, and making predictions.
Model Training: The linear regression model is trained on the training data, and predictions are made on the test data.
Visualization: The results are visualized by plotting the actual data points and the regression line, allowing you to assess how well the model fits both the training and test data.
This process demonstrates a basic application of supervised learning using simple linear regression. The visualizations help in understanding the model's performance on both the training and test sets.

Мета: Код спрямований на побудову простої лінійної регресійної моделі для прогнозування заробітної плати співробітника на основі його досвіду роботи (кількості років).

Обробка даних: Вона включає завантаження даних, їх поділ на навчальну та тестову вибірки, навчання моделі та здійснення прогнозів.

Навчання моделі: Лінійна регресійна модель навчається на навчальних даних, а потім використовується для прогнозування на тестових даних.

Візуалізація: Результати візуалізуються за допомогою графіків, де відображаються фактичні дані та лінія регресії, що дозволяє оцінити, наскільки добре модель відповідає як навчальним, так і тестовим даним.

Цей процес демонструє базове застосування методу з підконтрольним навчанням (supervised learning) за допомогою простої лінійної регресії. Візуалізації допомагають зрозуміти продуктивність моделі як на навчальній, так і на тестовій вибірці.

# Simple Linear Regression

Simple Linear Regression is a fundamental machine learning method used to model the relationship between two variables: an independent variable (input) and a dependent variable (output). The primary goal is to determine a line that best fits the data, enabling predictions of the dependent variable based on the independent variable.

## Purpose
- **Prediction**: Simple Linear Regression is used to predict the value of a dependent variable using the value of an independent variable. For example, predicting an employee’s salary based on their years of experience.
- **Relationship Analysis**: This method helps to understand whether a linear relationship exists between two variables and the strength of that relationship.
- **Trend Analysis**: It's useful for identifying trends and patterns in data, such as how sales vary over time.

## Applications
- **Economics**: Forecasting economic indicators like product demand based on variables such as price or income.
- **Finance**: Estimating asset values or predicting investment returns.
- **Social Sciences**: Analyzing the impact of one variable on another, such as the effect of education level on income.
- **Business Analytics**: Understanding the factors that influence sales or consumer behavior.

## Key Concepts
- **Simplicity**: Simple Linear Regression considers only one independent variable, making it the simplest form of regression analysis.
- **Linear Relationship**: The model assumes that there is a linear relationship between the independent and dependent variables, meaning that changes in one variable proportionally affect the other.
- **Regression Equation**: The regression line is described by the equation:
  \[
  y = b_0 + b_1x
  \]
  where:
  - \( y \) is the dependent variable (output)
  - \( x \) is the independent variable (input)
  - \( b_0 \) is the y-intercept (the point where the line crosses the y-axis)
  - \( b_1 \) is the slope of the line (the rate of change of the dependent variable with respect to the independent variable)
- **Accuracy Assessment**: It's essential to evaluate the model's fit using metrics such as the coefficient of determination (\( R^2 \)), which indicates the proportion of the variance in the dependent variable that is predictable from the independent variable.

## Summary
Simple Linear Regression is a crucial tool in data analysis and machine learning. Its simplicity and interpretability make it a foundational concept, important for understanding more advanced techniques in predictive modeling and data science.

# Проста лінійна регресія

Проста лінійна регресія — це базовий метод машинного навчання, який використовується для моделювання взаємозв'язку між двома змінними: незалежною змінною (вхідною) та залежною змінною (вихідною). Основна мета полягає в тому, щоб визначити лінію, яка найкраще відповідає даним, що дозволяє прогнозувати значення залежної змінної на основі незалежної змінної.

## Мета
- **Прогнозування**: Проста лінійна регресія використовується для прогнозування значення залежної змінної на основі значення незалежної змінної. Наприклад, прогнозування заробітної плати співробітника залежно від його досвіду роботи.
- **Аналіз взаємозв'язку**: Цей метод допомагає зрозуміти, чи існує лінійний зв'язок між двома змінними та наскільки цей зв'язок сильний.
- **Аналіз трендів**: Придатний для виявлення трендів і закономірностей у даних, наприклад, як змінюються обсяги продажу з часом.

## Застосування
- **Економіка**: Прогнозування економічних показників, таких як попит на продукцію, залежно від таких змінних, як ціна або дохід.
- **Фінанси**: Оцінка вартості активів або прогнозування доходності інвестицій.
- **Соціальні науки**: Аналіз впливу однієї змінної на іншу, наприклад, вплив рівня освіти на дохід.
- **Бізнес-аналітика**: Визначення факторів, які впливають на продажі або поведінку споживачів.

## Ключові концепції
- **Простота**: Проста лінійна регресія враховує лише одну незалежну змінну, що робить її найпростішою формою регресійного аналізу.
- **Лінійний зв'язок**: Модель передбачає, що між незалежною та залежною змінними існує лінійний зв'язок, тобто зміни в одній змінній пропорційно впливають на іншу.
- **Рівняння регресії**: Лінія регресії описується рівнянням:
  \[
  y = b_0 + b_1x
  \]
  де:
  - \( y \) — залежна змінна (вихід)
  - \( x \) — незалежна змінна (вхід)
  - \( b_0 \) — інтерцепт (точка перетину лінії з віссю y)
  - \( b_1 \) — нахил лінії (швидкість зміни залежної змінної стосовно незалежної змінної)
- **Оцінка точності**: Важливо оцінювати відповідність моделі за допомогою таких метрик, як коефіцієнт детермінації (\( R^2 \)), який вказує на частку дисперсії залежної змінної, що передбачувана за допомогою незалежної змінної.

## Резюме
Проста лінійна регресія є важливим інструментом у аналізі даних та машинному навчанні. Її простота та інтерпретованість роблять її фундаментальною концепцією, важливою для розуміння більш складних методів у прогностичному моделюванні та науці про дані.
