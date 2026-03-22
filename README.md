# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
 Include the necessary coding and corresponding screenshots
```
import seaborn as sns
import matplotlib.pyplot as plt

df=sns.load_dataset("iris")
corr_matrix=df.select_dtypes(include=["float64"]).corr()
sns.heatmap(corr_matrix, annot=True, cmap="coolwarm")
plt.show()

sns.jointplot(x='sepal_length',y='sepal_width',data=df,kind='hex')

sns.jointplot(x='sepal_length',y='sepal_width',data=df,kind='reg')

sns.pairplot(df)

sns.pairplot(df,hue='species')

sns.distplot(df['sepal_width'])

sns.distplot(df['petal_length'],kde=False,bins=10)

sns.countplot(x='species',data=df)

sns.countplot(y='species',data=df)

sns.barplot(x='sepal_length',y='sepal_width',data=df)

sns.boxplot(x='sepal_length',y='sepal_width',data=df)

sns.boxplot(x='sepal_length',y='sepal_width',data=df,palette='rainbow')

sns.boxplot(data=df,orient='v')

sns.boxplot(x='sepal_length',y='sepal_width',data=df,hue='species')

sns.violinplot(x='sepal_length',y='sepal_width',data=df,palette='rainbow')
```

#output
<img width="720" height="435" alt="Screenshot 2026-03-22 175716" src="https://github.com/user-attachments/assets/df450b89-927e-4e6b-bdab-e5785106c354" />
<img width="673" height="613" alt="Screenshot 2026-03-22 175723" src="https://github.com/user-attachments/assets/e2906cd1-a717-421a-8707-68bccbfca153" />
<img width="612" height="610" alt="Screenshot 2026-03-22 175731" src="https://github.com/user-attachments/assets/1220e047-3a11-48a5-83a6-13b8a6f99db1" />
<img width="691" height="530" alt="Screenshot 2026-03-22 175738" src="https://github.com/user-attachments/assets/4006be69-9072-4134-8930-635647dbedbd" />
<img width="665" height="544" alt="Screenshot 2026-03-22 175746" src="https://github.com/user-attachments/assets/c55c9b9e-8c60-4af4-b049-db3bdc24f314" />
<img width="600" height="484" alt="Screenshot 2026-03-22 175751" src="https://github.com/user-attachments/assets/1be5c97d-9a1a-4c62-8ea4-7d1ee07c1b19" />
<img width="667" height="528" alt="Screenshot 2026-03-22 175758" src="https://github.com/user-attachments/assets/cb2fd66a-a9e1-4719-98e7-1d8e3dd6319c" />
<img width="700" height="508" alt="Screenshot 2026-03-22 175804" src="https://github.com/user-attachments/assets/5ec2e166-ccc7-4023-8d0c-413d9deac5c8" />
<img width="670" height="495" alt="Screenshot 2026-03-22 175813" src="https://github.com/user-attachments/assets/d1619f58-0303-4e8f-b0c5-5b342e739b24" />
<img width="720" height="535" alt="Screenshot 2026-03-22 175853" src="https://github.com/user-attachments/assets/b13c60c2-d7dd-4cba-b381-30f473b0ac29" />
<img width="648" height="503" alt="Screenshot 2026-03-22 175900" src="https://github.com/user-attachments/assets/7cbb1f66-fdeb-4b0f-a976-97dad1de7dc1" />
<img width="655" height="507" alt="Screenshot 2026-03-22 175907" src="https://github.com/user-attachments/assets/29ed0a6c-facc-4585-95ef-7d58c591ece5" />
<img width="679" height="516" alt="Screenshot 2026-03-22 175913" src="https://github.com/user-attachments/assets/7f97f942-d3b4-4ac7-8c41-5225541ea362" />
<img width="766" height="716" alt="Screenshot 2026-03-22 175921" src="https://github.com/user-attachments/assets/c21f68ec-7a14-459f-a5e9-a8d29a233afe" />

<img width="764" height="725" alt="Screenshot 2026-03-22 175928" src="https://github.com/user-attachments/assets/514acecb-861c-4763-aebf-122723ea9691" />






# Result:
 Include your result here
Data Visualization using seaborn python library is verified successfully
