###Json 有关关键部分解答###

##1、查询返回结果为Json格式，没有序列化出现
`{create_date:1391141532000,...}`
出现该种情况，前端就不能正常展示，建议使用fastJson.jar 实现日期序列化
	
	@JSONField(format="yyyy/MM/dd")//保证前端数据的格式化正确
	@Temporal(TemporalType.DATE)
	@Column(name = "BUY_DATE", length = 7)
	


