# agile-git


##### Reading
[What happens when you press play?](http://highscalability.com/blog/2017/12/11/netflix-what-happens-when-you-press-play.html)

This is a long article, but a very interesting one since it talks about the architecture of Netflix and how they creatively tackled problems along the way. One of my favorite solutions out of many in their architecture is the way they tackled video networking. Instead of supplying the videos from datacenters to users, they have a specialized Content Delivery Network based on OCA's (Open-Connect-Appliances, native to Netflix) in partnership with Internet Service Providers (ISPs) and Internet Exchange Locations (IXPs). Since Netflix amounts to 37% of the internet traffic within the United States, Netflix’s OCAs are provided to ISPs and placed at or near IXP's. This benefits both Netflix, and IXP's and ISP's because it takes away the cost for IXP's and ISP's of fetching videos from Netflix's OSAs (reducing traffic flow) and provides Netflix to create a more seamless experience for the users. This solution is absolutely genius and unconventional, but only possible because of Netflix's huge share in the internet traffic.