# B站
> https://www.bilibili.com/

## 数据结构

```
mid:   用户id
name:  用户名
face:  用户头像url  noface.jpg为默认头像
sign： 签名

level: b站等级
coins: b站硬币
```

## 粉丝

```
https://api.bilibili.com/x/relation/fans?vmid={mid}&pn={pn}&ps={limit}&order=desc&gaia_source=main_web&web_location={web_location}&w_rid={wrid}&wts={wts}


获取指定mid（用户ID）的最新粉丝列表。  
:param mid: 用户ID，表示要查询mid的粉丝。  
:param pn: 页码，表示要查询的粉丝列表的页码。  
:param limit: 页面大小，即每页显示的粉丝数量。默认为20。
:param web_location: 默认为 1550101。
:param wrid: 网络参数
:param wts: 当前毫秒数 
:return: 返回一个包含最新粉丝信息的列表（具体返回格式取决于数据源）。  
```

## 关注


```
https://api.bilibili.com/x/relation/followings?vmid={mid}&pn=1&ps={limit}&order=desc&gaia_source=main_web&web_location={web_location}&w_rid={wrid}&wts={wts}

获取mid的最新关注。
参数同上
```

## 个人信息

```
https://api.bilibili.com/x/space/wbi/acc/info?mid={mid}&token=&platform=web&web_location={web_location}&dm_img_list={dm_img_list}dm_img_str={dm_img_str}&dm_img_inter={dm_img_inter}&w_rid={wrid}&wts={wts}

获取mid的个人信息。
:param dm_img_str: 可默认为 "V2ViR0wgMS4wIChPcGVuR0wgRVMgMi4wIENocm9taXVtKQ"。
:param dm_cover_img_str: 可默认为 "QU5HTEUgKEludGVsLCBJbnRlbChSKSBVSEQgR3JhcGhpY3MgNjMwICgweDAwMDAzRTlCKSBEaXJlY3QzRDExIHZzXzVfMCBwc181XzAsIEQzRDExKUdvb2dsZSBJbmMuIChJbnRlbC"。
:param dm_img_inter: 可默认为 "{\"ds\":[],\"wh\":[3256,5442,64],\"of\":[495,990,495]}"。
```


