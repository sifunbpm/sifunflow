sifunflow
=========

sifunflow 工作流引擎

SifunFlow工作流引擎采用微内核的架构。微内核架构的工作流引擎，将一些复杂的流程业务性问题，诸如组织人员任务分配，分支条件计算，事件操作，业务工作项的处理，业务数据保存，以及那些复杂的重新起草，退回，会签等，从工作流引擎中剥离出来，流程引擎关心的内容只是如何让一个流程按照预先定义的秩序从一个节点（状态）变换到另外一个节点（状态），而将上述的这些功能通过扩展的接口进行实现，并整合到流程引擎的内核中。
	技术体系
SifunFlow基于Domino开发，流程核心使用LotusScript编写，前端页面基于Dojo框架编写，设计灵活，易于扩展。如下图：
 

模块设计
SifunFlow主要基于流程库、人员组织库、核心应用库日志库等设计而成，各模块高内聚，低耦合，便于拆分，便于维护。如下图：
 

流程设计
SifunFlow流程需要经过创建、配置、流转审批、归档这几个步骤，下图可以形象的表述这一过程。
 
SifunFlow的流程表单采用轻量级设计，各流程组件通过流程表单的UNID唯一联系起来
 


