#### DATAFLOW操作说明

具体介绍Action, Workflow, Task的操作。

**Action**:

定义了可执行的动作。可以是shell/java/python脚本。

**Workflow:**

定义了一个可执行的workflow，包括多个action的有向无环图。定义了action之间的依赖关系。

**Task:**

Workflow定义好，通过cron定时执行，一次执行就是一个task。Task是可控的，用户可以暂停／重启／删除task。如果task处于非结束状态，即：失败或者暂停，cron启动的下次任务将不会被执行，直到task执行成功或者被删除。



