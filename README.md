# coverless-_detection
experimental result
### 文件说明
* .png文件为论文中实验结果表格
* baidunet.txt为具体的数据，由于数据量过大，没法上传GitHub，转储至百度网盘。数据包含了融合特征在数据集大小为2的10次方、2的14次方、2的18次方的情况下，对SIFT_BOF SIFT_HASH PIXEL CIHDN DCT_LDA FAST_RCNN六种隐写方案的检测结果。
### 百度网盘中实验数据文件名命名规则
* 正常用户文件命名规则："nor_users_pics_path" + "数据集大小" + ".txt"
* 隐写者文件命名规则："f_coverless_pics" + "检测图片数量" + "test" + "隐写方案" + "数据集大小" + ".txt"
### 百度网盘中实验数据的结构
* 实验结果文件内容结构：
* 正常用户的数据结构：

```
    for exp_times:
        for mess_len_list:
            for users:
                    (...)
```


> 如图所示：
> ![图片](https://user-images.githubusercontent.com/77422731/209758085-920ddbee-6bc7-489f-99e9-ba530e5737fb.png)
* 隐写者实验数据结构

```
    for exp_times:
        for users:
            f.write(mess)
        (...)
        for user:
            f.write(pics_path)
        (...)
        f.write(test_feature, test_lable)
```


![图片](https://user-images.githubusercontent.com/77422731/209758397-253cc47e-4258-44df-8ccf-2ac7c9a9a7ee.png)
![图片](https://user-images.githubusercontent.com/77422731/209758795-167b827d-68b7-45f8-b6cf-ee3f061b2ec6.png)


