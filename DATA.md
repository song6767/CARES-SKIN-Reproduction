# CARES 数据获取与本地使用

数据来源：[CARES-eskin/StressData](https://github.com/CARES-eskin/StressData)。原论文的[数据可用性说明](https://doi.org/10.1038/s41928-023-01116-6)指向该仓库。

## 本地目录约定

建议把作者数据仓库放在本项目目录的旁边：

```text
工作目录/
├── CARES_SKIN/          # 作者数据仓库；含 RawData/、DataAlignedForML/
└── CARES_SKIN_REPRO/    # 本复现仓库；只含自己的代码与说明
```

如果尚未下载，先在本项目的**上一级目录**执行：

```powershell
git clone https://github.com/CARES-eskin/StressData.git CARES_SKIN
```

本机已经有作者数据时，直接使用现有目录即可。后续代码应通过可配置的数据目录读取它；不要将数据文件复制进本仓库。`.gitignore` 也会拦截常见数据目录和数据文件扩展名，但提交前仍应检查 `git status`。

公开实验结果时，请引用原论文与数据仓库，并记录所用数据版本、标签定义和受试者划分。若需要在自己的仓库重新分发原始数据，应先确认原始权利人的明确授权。
