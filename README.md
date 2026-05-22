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
```
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df=pd.read_csv("titanic_dataset.csv")
df.head()
 x=[1,2,3,4,5]
 y=[3,6,2,7,1]
 sns.lineplot(x=x,y=y)
 plt.title('Line Plot')
 x=[1,2,3,4,5]
 y1=[3,5,2,6,1]
 y2=[1,6,4,3,8]
 y3=[5,2,7,1,4]
 sns.lineplot(x=x,y=y1)
 sns.lineplot(x=x,y=y2)
 sns.lineplot(x=x,y=y3)
 plt.title('Multi Line Plot')
 plt.figure(figsize=(8,5))
 sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
 plt.title("Fare Of Passenger By Embarked Town")
 sns.scatterplot(x="Age", y="Fare", data=df)
 plt.title('Scatterplot of Age vs Fare')
 plt.show()
 sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
 plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
 plt.show()
 sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
 sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
 plt.title("Age By Passenger Class")
sns.kdeplot(data=df['Age'], shade=True)
 plt.title('Density Plot of Passenger Ages')
 plt.show()
  numeric_df = df.select_dtypes(include=['float64', 'int64'])
 corr_matrix = numeric_df.corr()
 sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
 plt.title('Heatmap of Titanic Dataset')
 plt.show()
```
<img width="1618" height="281" alt="Screenshot 2026-05-22 112729" src="https://github.com/user-attachments/assets/1fc37a5f-7f08-49c7-9e49-413c6993c214" />
<img width="1095" height="815" alt="Screenshot 2026-05-22 112746" src="https://github.com/user-attachments/assets/ec952546-2504-4067-9b61-e6fb0c1e429c" />
<img width="801" height="609" alt="Screenshot 2026-05-22 112802" src="https://github.com/user-attachments/assets/85c750d0-9736-4f74-af56-45612c227f8f" />
<img width="1001" height="680" alt="Screenshot 2026-05-22 112823" src="https://github.com/user-attachments/assets/cc133c7d-6332-42c4-8088-938502091ee3" />
<img width="817" height="585" alt="Screenshot 2026-05-22 112838" src="https://github.com/user-attachments/assets/c82b6eab-68e4-4df7-92c9-4370ccbc1e20" />
<img width="811" height="580" alt="Screenshot 2026-05-22 112918" src="https://github.com/user-attachments/assets/aa03cd2c-b3a3-4ad2-ad9b-43d2b7fee67c" />
<img width="823" height="555" alt="Screenshot 2026-05-22 112942" src="https://github.com/user-attachments/assets/7aa68523-c2b8-4f94-b43b-e0c5b2733c84" />
<img width="996" height="771" alt="Screenshot 2026-05-22 113009" src="https://github.com/user-attachments/assets/81891c8b-ac9a-4c09-b9a1-a15f326d9fd9" />
<img width="779" height="571" alt="Screenshot 2026-05-22 113025" src="https://github.com/user-attachments/assets/0606cab8-35b0-400a-8262-1d7b418fd97b" />
<img width="788" height="589" alt="Screenshot 2026-05-22 113041" src="https://github.com/user-attachments/assets/4dcd4ea7-bb59-4000-a6bc-46cceb3a9d54" />
<img width="757" height="648" alt="Screenshot 2026-05-22 113059" src="https://github.com/user-attachments/assets/d5e016ef-4ac8-4aa6-843c-0046e20710d2" />

 # Result:
Thus, the Data Visualization using seaborn python library for the given data is implemented successfully
