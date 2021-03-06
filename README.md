# chamc-workflow-releaseNotes

请查看repository-release note，或参考以下内容。

## 3、新增接口 ##

2018/2/24 15:50:48

#### 开发平台-工作流模块（bpm） ####

> - 增加查询待办已办接口，入参均为（QueryTaskParam param, Pageable pageable），构造QueryTaskParam时通过工厂函数构造，且可以通过流式api设置属性值
> QueryTaskParam可设置属性：userId、taskId、processDefineKeys[list]、processTitle
> - 同组织的支持(启动时传入提交人部门id，在后面的节点设置参与人为制单人同组织+角色，可根据部门自动找到同组织下的用户)
>
>- 参考信息：[开发平台后端框架参考指南-流程引擎模块](http://hq-spsdocument/_layouts/15/DocIdRedir.aspx?ID=C2A742TNNUZA-1797567310-1214)

## 2、新增接口 ##

2018/2/1 16:05:23

#### 开发平台-工作流模块（bpm） ####

> - 增加任务操作相关接口：查询待办数量、根据processKey查询待办/已办、驳回到指定节点
> 
>- 参考信息：[开发平台后端框架参考指南-流程引擎模块](http://hq-spsdocument/_layouts/15/DocIdRedir.aspx?ID=C2A742TNNUZA-1797567310-1214)

#### 工作流平台 ####

初始化工作流引擎基础框架支持

> - 根据processKey查询的支持
> - 同组织/同机构时选人的问题修复
>
> - 参考信息：[统一流程引擎平台介绍](http://hq-spsdocument/_layouts/15/DocIdRedir.aspx?ID=C2A742TNNUZA-1797567310-1222)

## 1、初始化新建项目 ##

2018.01.22

#### 开发平台-工作流模块（bpm） ####

> - 增加流程实例相关接口：启动流程、查询流转明细、查询流程变量、查询流程实例（根据key）
> - 增加任务操作相关接口：查询待办/已办列表、根据taskId查询待办/已办
> 
> - 增加任务操作的监听处理`BpmOperateListener`
> 
> - 增加工作流同步程序
>- 参考信息：[开发平台后端框架参考指南-流程引擎模块](http://hq-spsdocument/_layouts/15/DocIdRedir.aspx?ID=C2A742TNNUZA-1797567310-1214)

#### 工作流平台 ####

初始化工作流引擎基础框架支持

> - 增加流程管理台页面
> - 增加常见接口调用
> 
> - 增加特殊场景支持：同机构/部门+角色的人员限定、并行/串行会签、多租户、人员兼职、驳回到组/人等
> - 参考信息：[统一流程引擎平台介绍](http://hq-spsdocument/_layouts/15/DocIdRedir.aspx?ID=C2A742TNNUZA-1797567310-1222)
