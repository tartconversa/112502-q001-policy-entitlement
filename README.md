# 惠企免申政策的资格认定与资金兑现

本项目用于整理相关业务资料。CSV 文件采用 UTF-8 编码，首行为字段名，日期使用 ISO 格式；空单元格表示来源未提供。样例记录为合成数据。

## 样例资料

- `enterprises.csv` 包含样例字段 `enterprise,department,industry_code,valid_from,valid_to,region`。
- `policies.csv` 包含样例字段 `policy,version,industry_code,effective_from,effective_to,rate,cap`。
- `bills.csv` 包含样例字段 `bill,enterprise,period_start,period_end,amount,revision`。
- `payments.csv` 包含样例字段 `payment,enterprise,policy,bill,amount,state,decision_version`。

## 运行检查

需要 Python 3.11 或更高版本，无第三方依赖。

```bash
python3 -m unittest discover -s tests -v
python3 -m compileall -q tests
```
