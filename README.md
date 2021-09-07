# Analysis of vacancies on hh.ru

This project helps to extract important facts from the raw text of hh.ru vacancies in the IT segment of the market. With the help of it, you can get a set of required skills, a set of nice-to-have skills, you can extract the name of the sub-area of a given vacancy and other useful facts. 

## Example of usage

This part of code shown in the bottom of `facts_extraction.ipynb`:

```
# input here id of any vacancy on hh.ru
vacancy_id = 45191074

# then get it's facts extracted
print(extract_facts_from_vacancy(vacancy_id))
```

Result:
```
{
    'Обязательные компетенции': ['Python', 'NumPy', 'Scikit', 'Работа с базами данных', 'A', 'XGBoost', 'SQL', 'Математический анализ', 'аналитика', 'Математическая статистика', 'Plotly', 'Информационные технологии'], 
    'Желательные компетенции': ['Нейросети', 'PyTorch'], 
    'Гибкий график работы': True, 
    'Подобласть': 'Data Science'
}
```
