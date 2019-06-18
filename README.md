# eccodes_supply_definitions

> 本项目由个人开发，非官方提供，如有问题，请尽量自行解决

eccodes补充grib定义

## 1. 缘起
eccodes在用于读取业务化的国内GRIB2数据，如中央台数据、华东区域模式数据时，
会出现许多的shortName为unknown的情况，对于多个unknown变量的GRIB2文件，
往往需要通过多种过滤手段逐步确定变量具体是什么，区分它们令人沮丧。


## 2. 进度

2019.6.18 支持华东区域模式地面输出GRIB2文件（文件名形如：Z_NAFP_C_BCSH_20190611120000_P_surface-warms-f12.BIN）

## 3. 使用

1. 修改 eccodes目录下的definitions/common/c-11.table文件，在 `38 babj Beijing (RSMC)` 下增加一行 `39 bcsh Shanghai`
2. 将本工程下的 `bcsh` 目录放到 definitions/grib2/localConcepts 目录下


## 4. 丰富

- 完善支持更多国产数据