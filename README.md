# User KiCad Symbols（KiCad用户符号库）

## 创立原因
- 由于合并请求提交后，需要一段时间来等待管理员审核通过，并且在这一期间内，根仓库中不含有新增的符号，所以我创立了该项目。

## 目的
- 统计并管理那些已经提交、并且还未被审核员批准通过的合并请求。

## 库存放位置
- 这些库应该放到KiCad的用户库路径下，并且添加软件内的索引路径。

    备注：如果找不到用户库路径，请参见[KiCad官网帮助页面](https://docs.kicad.org/8.0/zh/getting_started_in_kicad/getting_started_in_kicad.html) 寻找答案。

## 命名规则
- [√] 符号命名：完全遵循KiCad符号库命名规范，并且经过klc-check校验。
- [√] 符号库命名：在复制（复制将要与目标库合并的源库到用户库路径下）后的命名最前端增加“User_”字符串。

## 生命周期
1. 当合并请求被管理员审核通过、并且该符号库新增符号已经被添加进根符号库后，本项目内的对应用户符号库将会被删除。
2. 而后，用户应手动删除KiCad的用户库路径下的对应符号库。
3. 最终，从[KiCad符号库项目](https://gitlab.com/kicad/libraries/kicad-symbols)下载最新的根符号库并将软件本体的符号库覆盖。
