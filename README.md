## 自动下载youtube视频,上传到头条系统

### 需要安装 shadowsocks, youtube-dl 

### 使用方式

1.浏览器访问index.php把需要下载的youtube视频地址录入数据库

2.浏览器访问code.php把获取头条token到数据库[只需一次]

3.添加计划任务 [每小时执行]
```$xslt
0 */1 * * * *  /usr/bin/php  /home/wwwroot/zgq.hanhanjun.com/dl.php > /dev/null 2>&1 &
```

4.登录头条后台: 内容管理->草稿中修改信息发布