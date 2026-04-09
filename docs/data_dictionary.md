# H&M数据字典

## 1. articles.csv（商品信息，约10万条）
| 字段 | 含义 | 用途 |
|------|------|------|
| article_id | 商品ID | 主键 |
| product_code | 产品编码 | 聚合同款不同色 |
| product_type_name | 产品类型（T恤、裤子等） | 特征工程 |
| product_group_name | 产品组（上衣、下装等） | 类别特征 |
| graphical_appearance_name | 图案（纯色、条纹等） | 视觉特征 |
| colour_group_name | 颜色 | 用户偏好 |
| department_name | 部门 | 商品层级 |
| index_name | 索引分类（女装、男装等） | 大类划分 |
| index_group_name | 索引组 | 更粗粒度分类 |
| section_name | 区域 | 场景特征 |
| garment_group_name | 服装组 | 穿搭场景 |

## 2. customers.csv（用户信息，约136万人）
| 字段 | 含义 | 用途 |
|------|------|------|
| customer_id | 用户ID | 主键 |
| FN | 是否接收新闻通讯 | 活跃度特征 |
| Active | 是否活跃 | 用户分层 |
| club_member_status | 会员状态 | 忠诚度 |
| fashion_news_frequency | 时尚资讯频率 | 兴趣度 |
| age | 年龄 | 核心画像特征 |
| postal_code | 邮编 | 地区特征 |

## 3. transactions_train.csv（交易记录，约1.3亿条）
| 字段 | 含义 | 用途 |
|------|------|------|
| t_dat | 交易日期 | 时间序列特征 |
| customer_id | 用户ID | 关联用户 |
| article_id | 商品ID | 关联商品 |
| price | 价格 | 消费力特征 |
| sales_channel_id | 销售渠道（1=线上，2=线下） | 渠道偏好 |

## 4. sample_submission.csv（提交格式）
- 每行：customer_id + 12个推荐的article_id（空格分隔）