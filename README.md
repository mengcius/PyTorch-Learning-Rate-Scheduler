## PyTorch学习率调整策略
PyTorch中学习率调整策略通过 torch.optim.lr_scheduler 接口实现，一共9种方法，可分为三大类：

a. 有序调整：等间隔Step调整、指定多间隔MultiStep调整学习率、指数衰减调整Exponential、余弦退火CosineAnnealing

b. 自适应调整：自适应调整ReduceLROnPlateau

c. 自定义调整：自定义lamda调整LambdaLR

torch.optim.lr_scheduler.LambdaLR 自定义lamda函数
torch.optim.lr_scheduler.StepLR 等间隔阶梯下降
torch.optim.lr_scheduler.MultiStepLR 指定多间隔step_list阶梯下降
torch.optim.lr_scheduler.ExponentialLR 指数下降
torch.optim.lr_scheduler.CosineAnnealingLR 余弦退火
torch.optim.lr_scheduler.CosineAnnealingWarmRestarts 带热启动的余弦退火
torch.optim.lr_scheduler.CyclicLR 循环调整
torch.optim.lr_scheduler.OneCycleLR 第一次退火到大学习率
torch.optim.lr_scheduler.ReduceLROnPlateau 自适应下降
