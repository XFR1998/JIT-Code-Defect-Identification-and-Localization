# 😄Recore my study note of code defect identification and localization


# JIT数据集
## 🚀1.OPENSTACK（C++）  
train: 11973 (阳：1464)  
test: 1331 (阳：163)  
all: 13304 (阳：1627)  
## 🚀2.QT（C++）  
train: 23133 (阳：1642)  
test: 2571 (阳：183)    
all: 25704 (阳：1825)  

其中：    
**_train.pkl, _test.pkl内数据含义：**  
len(df) = 4   
df[0]: commit id  
df[1]: defect label  
df[2]: commit msg  
df[3]: added_code, removed_code for each commit  


**_train_dextend.pkl, _test_dextend.pkl内数据含义：**  
len(df) = 4  
df[0]: commit id  
df[1]: defect label  
df[2]: commit msg  
df[3]: "added_code removed_code" for each commit  

**_dict.pkl内数据含义：**   
有2个字典：  
dict[0]: commit_msg的dict  
dict[1]: code的dict  

**_train_cc2ftr.pkl, _test_cc2ftr.pkl内数据含义：**  
cc2vec模型的向量特征：code changes features

**⭐如下论文对这个数据集做了扩充，并增多了4个项目：**  
**(ISSTA-2021) 《Deep Just-in-Time Defect Prediction How Far Are We？》**
![image](https://user-images.githubusercontent.com/65661019/156569647-01fab139-cac2-4a1f-88e1-3c87451d92aa.png)




