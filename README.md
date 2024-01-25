# Image Classification Benchmarks

## 安装必备的环境
    pip install -r requirements.txt

## 安装可视化可视化工具
    pip install wandb


## 开始训练

### Single GPU
    python train.py root '数据集的路径' devide 'cuda:0'(如果有的话)

### 保留可视化结果
    在train.py文件下
    os.environ["WANDB_API_KEY"] = 你的wandb-KEY
    os.environ["WANDB_MODE"] = "offline"
    wandb.init()
    wandb.finish()
