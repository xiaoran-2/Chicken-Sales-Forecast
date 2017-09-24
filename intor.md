from sklearn import linear_model
regr = linear_model.LinearRegression()
regr.fit(x, y)
This model sourec is 0.215982034941


# 默认max_iter = 500
regr = linear_model.LassoLars(alpha = 0.1)
regr.fit(x, y)
This model sourec is 0.143395842152

regr = linear_model.LassoLars(alpha = 0.5)
regr.fit(x, y)
This model sourec is 0.143395842152


regr = linear_model.LassoLars(alpha = 0.01)
regr.fit(x, y)
This model sourec is 0.142976810521

regr = linear_model.LassoLars(alpha = 0.01,max_iter = 1000)
regr.fit(x, y)
This model sourec is 0.142976810521


regr = linear_model.ElasticNet()
regr.fit(x, y)
This model sourec is 0.143374608153


#最优结果0
regr = linear_model.ElasticNetCV()
regr.fit(x, y)
This model sourec is 0.134310413311

#增加skew偏度特征后的结果。不明显
regr = linear_model.ElasticNetCV()
regr.fit(x, y)
This model sourec is 0.134310844858

#增加skew偏度和均值特征后的结果。
This model sourec is 0.134311153881


regr = KernelRidge()
regr.fit(x, y)
This model sourec is 0.302077966324

# 对最优的模型，修改参数，不要全部修改，尝试微调
# 默认参数 l1_ratio=0.5, eps=0.001, n_alphas=100, max_iter=1000, tol=0.0001, n_jobs=1, 
regr = linear_model.ElasticNetCV(l1_ratio=0.1, eps=0.0001, n_alphas=120, max_iter=2000, tol=0.00001, n_jobs=4) # 修改参数，擦尝试结果
regr.fit(x, y)
This model sourec is 0.273805029557


regr = linear_model.ElasticNetCV(l1_ratio=0.7,tol=0.00001, n_jobs=4) # 修改参数，擦尝试结果
This model sourec is 0.136308424312


regr = linear_model.ElasticNetCV(l1_ratio=0.5,tol=0.0001, n_jobs=4) # 修改参数，擦尝试结果
This model sourec is 0.134465669656

regr = linear_model.ElasticNetCV(l1_ratio=0.5,eps=0.8,n_jobs=4) # 修改参数，擦尝试结果
This model sourec is 0.141910186614


# 最优结果，1,对应的结果文件result_ElasticNetCV1.csv
regr = linear_model.ElasticNetCV(l1_ratio=0.5,eps=0.01,max_iter=1000,n_jobs=4) # 修改参数，擦尝试结果
This model sourec is 0.128160018617

regr = linear_model.ElasticNetCV(l1_ratio=0.5,eps=0.01,max_iter=1500,n_jobs=4) # 修改参数，擦尝试结果
This model sourec is 0.12773133698

regr = linear_model.ElasticNetCV(l1_ratio=0.5,eps=0.01,max_iter=2500,n_jobs=4) # 修改参数，擦尝试结果
This model sourec is 0.128553124478

regr = linear_model.ElasticNetCV(l1_ratio=0.5,eps=0.01,max_iter=2000,n_jobs=4) # 修改参数，擦尝试结果
This model sourec is 0.128523613014


regr = linear_model.ElasticNetCV(l1_ratio=0.5,eps=0.01,max_iter=1600,n_jobs=4) # 修改参数，擦尝试结果
This model sourec is 0.128057615583

regr = linear_model.ElasticNetCV(l1_ratio=0.5,eps=0.01,max_iter=1200,n_jobs=4) # 修改参数，擦尝试结果
This model sourec is 0.128269958774



# ----------------------------------------------------------------------------------------
#最优结果0，对应的结果文件result_ElasticNetCV1.csv
regr = linear_model.ElasticNetCV()
regr.fit(x, y)
This model sourec is 0.134310413311


# 最优结果，1,对应的结果文件result_ElasticNetCV1.csv
regr = linear_model.ElasticNetCV(l1_ratio=0.5,eps=0.01,max_iter=1000,n_jobs=4) # 修改参数，擦尝试结果
This model sourec is 0.128160018617


# 最优参数，确定的参数，l1_ratio=0.5,eps=0.01,max_iter=1300,n_jobs=4，结果result_ElasticNetCV_2.csv'
regr = linear_model.ElasticNetCV(l1_ratio=0.5,eps=0.01,max_iter=1300,n_jobs=4) # 修改参数，擦尝试结果
This model sourec is 0.126494987321
结果得分：0.37717 


# 最优参数，确定的参数，l1_ratio=0.5,eps=0.01,max_iter=1300,n_jobs=4，结果result_ElasticNetCV_3.csv'
regr = linear_model.ElasticNetCV(l1_ratio=0.5,eps=0.01,max_iter=1300,n_jobs=4) # 修改参数，擦尝试结果
This model sourec is 0.126099597815
结果得分：？


# 明天尝试提交这个结果 result_LassoLars(alpha = 0.01).csv
regr = linear_model.LassoLars(alpha = 0.01)
regr.fit(x, y)
This model sourec is 0.142976810521




