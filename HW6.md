使用 UMLet 建模<br>

1、使用类图，分别对 Asg_RH 文档中 Make Reservation 用例以及 Payment 用例开展领域建模。然后，根据上述模型，给出建议的数据表以及主要字段，特别是主键和外键<br>
注意事项：<br>
对象必须是名词、特别是技术名词、报表、描述类的处理；<br>
关联必须有多重性、部分有名称与导航方向<br>
属性要注意计算字段<br>
数据建模，为了简化描述仅需要给出表清单，例如：<br>
Hotel（ID/Key，Name，LoctionID/Fkey，Address…..）<br><br>
2、使用 UML State Model，对每个订单对象生命周期建模<br>
建模对象： 参考 Asg_RH 文档， 对 Reservation/Order 对象建模。<br>
建模要求： 参考练习不能提供足够信息帮助你对订单对象建模，请参考现在 定旅馆 的旅游网站，尽可能分析围绕订单发生的各种情况，直到订单通过销售事件（柜台销售）结束订单。<br><br>

答:<br>
由HW5中的用例图以及文档中软件界面可知，<br>
Make Reservation中有关概念对象有：Hotel，Room，RoomDescription, Reservation, Reservation Item<br><br>
Hotel (HotelID/Key ,LocationID/Fkey, Name, Address, BriefIntroduction, MaxDiscount, StarsRating, Favorites, LowestPrice)<br>
Reservation (ReservationID/Key, Time, CheckInDate, CheckOutDate)<br>
ReservationItem (ReservationItemID/Key, Time, CheckInDate, CheckoutDate, Price, RoomNums, AdultNums, ChildNums, ChildAges)<br>
CustomerInfo(CustomerID/Key, Name, SpecialRequirement, IsSmoking)<br>
Room (RoomID/Key, Type, isAvailable, Price)<br>
Room-Description (RoomID/FKey, Type, Total, Price, Description)<br><br>
对Make Reservation开展领域建模：<br>
![image]()

对Payment开展领域建模：<br>
Payment中有关概念对象有:
