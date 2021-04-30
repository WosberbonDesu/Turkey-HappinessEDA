# HappinessEDA
### Visualization with seaborn for Happiness report 2021
You can arrange according to the country you want
I am writing the codes when you have to change, so you can get the data set you want
write the countries you want with the same number 
I made a visualization using middle east and north africa countries, you can do it according to northern europe south asia middle asia or america
![Ekran Alıntısı](https://user-images.githubusercontent.com/69467096/116694866-7798fb80-a9c8-11eb-8874-b615f7019d67.PNG)


```python

lel = ['Israel',
 'Bahrain',
 'Saudi Arabia',
 'Kuwait',
 'Libya',
 'Turkey',
 'Morocco',
 'Algeria',
 'Iraq',
 'Iran',]
 or
 lel = ['USA',
 'Uk',
 'Geramny',
 'France',
 'Italy',
 'Spain',
 'Greece',
 'Russia',
 'Poland',
 'Canada',]
```
change the country you want color to stand out by the first value
For example, among the countries you have listed, your country is in 3 rows, you can change it by typing three instead of 5.

```python

lel = ['Israel',
  bars1[5].set_alpha(1)
  bars1[5].set_color(colors_red[3])
  bars1[5].set_edgecolor(colors_dark[0])

```
If you want to make another comparison, the values ​​you need to change instead of ladder score:


```python
mean_score = data_2021['here'].mean()
bars0 = ax.bar(data_2021_top['Country name'], data_2021_top['HERE'], color=colors_blue[0], alpha=0.6, edgecolor=colors_dark[0])
bars1 = ax.bar(df['Country name'], df['HERE'], color=colors_dark[3], alpha=0.4, edgecolor=colors_dark[0])
bars2 = ax.bar(data_2021_bot['Country name'], data_2021_bot['HERE'], color=colors_red[0], alpha=0.6, edgecolor=colors_dark[0])
line  = ax.axhline(mean_score, linestyle='--', color=colors_dark[2])

```
