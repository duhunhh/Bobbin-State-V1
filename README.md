# Bobbin-State-V1 数据集

“Bobbin-State-V1” 是一个专为筒纱状态检测而构建的工业图像数据集。所有图像均通过部署在现代化纺织工厂测试车间内的在线图像采集系统获取，确保了数据的真实性和场景相关性。

## 1. 数据集构建

* **数据规模**：经过筛选和清理，数据集共包含 13,972 张高质量图像。
* **数据划分**：按照 8:1:1 的比例将数据集分为训练集、验证集和测试集。
    * **训练集**：11,178 张
    * **验证集**：1,398 张
    * **测试集**：1,398 张

## 2. 标注与类别

数据集根据纺纱过程的实际需求，严格定义了三种工业状态，并通过两个基础检测类别进行推断。

* **工业状态 (3种)**：
    1.  `No Bobbin`（无筒纱）
    2.  `Empty Bobbin`（空筒管）
    3.  `Yarn Bobbin`（满纱）

* **基础检测类别 (2类)**：
    1.  `Bobbin`（筒管）
    2.  `Yarn`（纱线）

## 3. 状态映射逻辑

三种工业状态是通过基础检测类别的组合来判定的：

* **No Bobbin**：模型未检测到任何目标（对应未标注图像）。
* **Empty Bobbin**：模型仅检测到 `Bobbin` 目标。
* **Yarn Bobbin**：模型同时检测到 `Bobbin` 和 `Yarn` 目标。

## 4. 数据统计

数据集中标注目标的统计数据如下：

| 类别 (Class) | 目标总数 (Total Instances) |
| :--- | :--- |
| `Bobbin` | 12,267 |
| `Yarn` | 6,535 |

*注：数据集中还包含 1,705 张未标注图像，这些图像对应 “No Bobbin” 状态。*
“Bobbin-State-V1” 是一个专为筒纱状态检测而构建的工业图像数据集。所有图像均通过部署在现代化纺织工厂测试车间内的在线图像采集系统获取，确保了数据的真实性和场景相关性。
数据集构建
数据规模：经过筛选和清理，数据集共包含 13,972 张高质量图像。
数据划分：按照 8:1:1 的比例将数据集分为训练集（11,178张）、验证集（1,398张）和测试集（1,398张）。
标注与类别：数据集根据纺纱过程的实际需求，严格定义了三种工业状态：“No Bobbin”（无筒纱）、“Empty Bobbin”（空筒管）和 “Yarn Bobbin”（满纱）。
为了实现这三种状态的检测，标注阶段定义了两个基础检测类别：“Bobbin”（筒管）和 “Yarn”（纱线）。
状态映射逻辑：
No Bobbin：模型未检测到任何目标。
Empty Bobbin：模型仅检测到 “Bobbin” 目标。
Yarn Bobbin：模型同时检测到 “Bobbin” 和 “Yarn” 目标。
数据统计：数据集中总共标注了 12,267 个 “Bobbin” 目标和 6,535 个 “Yarn” 目标（注：数据集中还包含 1,705 张未标注图像，对应 “No Bobbin” 状态）。
In addition, our data set is too large for you to download directly, we provide you with the following two download methods.
You can download the dataset from Quark Netdisk. URL：https://pan.quark.cn/s/fb9977b1d2b3. Extraction code: hEQP.
You can download the dataset from Baidu Netdisk. URL：https://pan.baidu.com/s/1laSbixrVfpY8rlt0Zl8eTg?pwd=egcf. Extraction code: egcf.

If you have any problem, please contact me by email：2024487434@qq.com.
