#说明
帮忙修改插件，加入一些filter；
ror的学习曲线太陡峭了，勉强调试通过。
修订清单：
/app/controllers/home_monitoring_controlling_project_controller.rb
/app/views/home_monitoring_controlling_project/_filters.html.erb

进度：
tag_tracker参数，修改values为id，可以成功传values，controllers接收参数并拼接成字符串，查询成功；
tag_issue_status参数，目前values还是汉字，暂未找到变更为id的 字段
checkbox及select的选择状态暂未控制，或可以通过js搞定；
页面上加上过滤器后，查询成功后部分title需要修改；

#测试链接
http://10.33.33.117:9988/home_monitoring_controlling_project/index/test1?utf8=%E2%9C%93&page=&filter_form_action=&field_tracker=1&tag_tracker%5B%5D=%E7%BC%BA%E9%99%B7&commit=%E5%BA%94%E7%94%A8#
#测试链接 ：
http://10.33.33.117:9988/home_monitoring_controlling_project/index/test1?utf8=%E2%9C%93&page=&filter_form_action=&field_tracker=1&tag_tracker%5B%5D=1&tag_issue_status%5B%5D=%E5%B7%B2%E5%AE%A1%E6%A0%B8&commit=%E5%BA%94%E7%94%A8#

#原始代码
the plugin source is : 
https://github.com/alexmonteiro/Redmine-Monitoring-Controlling