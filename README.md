# test
Markdown快速上手
查看源代码快捷键:Ctrl+/
# 1、标题

//标题一共有6个级别，书写方式如下：
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题


# 2、字体

//粗体
**你好呀，叶先森**

//斜体
*我喜欢你*

//删除线
此内容为废弃内容~~


# 3、引用

//引用书写语法如下：

>此教程来自叶十三出品，版权所有，违版必究
>>此教程来自小小叶儿出品，版权所有，违版必究
>>>此教程来自小小叶儿出品，版权所有，违版必究

# 4、分割线

//分隔线（长度：根据内容而定）
---
//分割线（占全屏）
***
# 5、图片

//图片插入
![图片名称](图片地址-可以本地：也可以网络)
5.1本地图片：

由于本地图片是在网页上是无法直接显示的，看语法就行
5.2网络图片：

图片
me
6、超链接

//超链接
[]

7、列表

//有序列表：序号+点+空格，生成列表 
1. 首页
2. 分类
3. Lll
//无需列表：- + 空格
- 

8、表格

//鼠标右键-->插入-->表格
名字	性别	生日
迪丽热巴	女	1991.1.1
9、代码

//代码块
`java --（名称）
package com.yrp.po;

import javax.persistence.*;
import java.util.ArrayList;
import java.util.Date;
import java.util.List;

@Entity
@Table(name = "t_user")
public class User {

    @Id
    @GeneratedValue
    private Long id;
    private String nickname;
    private String username;
    private String password;
    private String email;
    private String avatar;
    private Integer type;
    @Temporal(TemporalType.TIMESTAMP)
    private Date createTime;
    @Temporal(TemporalType.TIMESTAMP)
    private Date updateTime;

    @OneToMany(mappedBy = "user")
    private List<Blog> blogs = new ArrayList<>();

    public User() {
    }

    public Long getId() {
        return id;
    }

    public void setId(Long id) {
        this.id = id;
    }

    public String getNickname() {
        return nickname;
    }

    public void setNickname(String nickname) {
        this.nickname = nickname;
    }

    public String getUsername() {
        return username;
    }

    public void setUsername(String username) {
        this.username = username;
    }

    public String getPassword() {
        return password;
    }

    public void setPassword(String password) {
        this.password = password;
    }

    public String getEmail() {
        return email;
    }

    public void setEmail(String email) {
        this.email = email;
    }

    public String getAvatar() {
        return avatar;
    }

    public void setAvatar(String avatar) {
        this.avatar = avatar;
    }

    public Integer getType() {
        return type;
    }

    public void setType(Integer type) {
        this.type = type;
    }

    public Date getCreateTime() {
        return createTime;
    }

    public void setCreateTime(Date createTime) {
        this.createTime = createTime;
    }

    public Date getUpdateTime() {
        return updateTime;
    }

    public void setUpdateTime(Date updateTime) {
        this.updateTime = updateTime;
    }


