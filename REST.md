##### REST API 说明

DATAFLOW 提供了curl 的REST API ，可以用来创建action，删除action，修改action，查询action等，基于这些API，第三方系统可以与DATAFLOW紧密集成。

**添加 API**

请求方式 :POST

访问路径 

action : curl -d "action.name=test" http://host:port/action/save

workflow :curl -d "workflow.name=test" http://host:port/workflow/save

例：curl -d "action.name=test&action.desc=这是一个测试" http://10.1.1.70:1234/save

**修改API**

请求方式：POST

访问路径

action:curl -d "action.name=test01" http://host:port/action/update

workflow:curl -d "workflow.name=test01&workflow.cron=test02" http://host:port/workflow/update

例：curl -d "action.name=test01&action.desc=修改" http://10.1.1.70:1234/action/update

**查询API**

请求方式：GET

Action:curl http://host:port/action?name="test"

workflow:curl http://host:port/workflow?name="test"

taskHistory:curl http://host:port/taskHistory?name="test"

Task:curl http://host:port/task?name="test"

例：curl http://10.1.1.70:1234/action?name="test"

**删除API**

请求方式：GET

Action:curl http://host:port/action/testid

Workflow:curl http://host:port/workflow/testid

taskHistory:curl http://host:port/taskHistory/testid

Task:curl http://host:port/task/testid

例：curl http://10.1.1.70:1234/action/1011 



