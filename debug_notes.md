# 调试记录
1. 报错：CUDA out of memory
   原因：batch size 过大
   修改：batch_size=64

2. 报错：路径含中文无法加载数据
   原因：Windows 中文路径
   修改：代码目录改为全英文

3. 报错：维度不匹配
   原因：LeNet 需要 32×32 输入
   修改：添加 transforms.Resize((32,32))
