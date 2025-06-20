本教程将采用2025年5月20日正式的GA版，给出如下内容
1. 核心功能模块的快速上手教程
2. 核心功能模块的源码级解读
3. Spring ai alibaba增强的快速上手教程 + 源码级解读

版本：
- JDK21
- SpringBoot3.4.5
- SpringAI 1.0.0
- SpringAI Alibaba 1.0.0.2

### 项目目录结构
```text
chat目录                            
    - alibaba-chat                  # 基于alibaba实现chat案例
    - openai-chat                   # 基于openai实现chat案例
    - deepseek-chat                 # 基于deepseek实现chat案例
advisor目录                         
    - advisor-base                  # advisor绑定内存记忆案例
    - advisor-memory-sqlite         # 基于sqlite的advisor绑定内存记忆案例
    - advisor-memory-mysql          # 基于mysql的advisor绑定内存记忆案例
    - advisor-memory-redis          # 基于redis的advisor绑定内存记忆案例
tool-calling                        # 时间、天气两个工具的function、method调用案例
structured-output                   # map、list、实例对象类型的格式化输出案例
vector目录                         
    - vector-simple                 # 基于内存的向量数据库案例
    - vecotr-redis                  # 基于redis的向量数据库案例
    - vector-elasticsearch          # 基于ES的向量数据库案例
rag目录                             
    - rag-simple                    # 基于内存的rag效果对比、模块化rag案例
    - rag-etl-pipeline              # 提取文档、转换文档、写出文档的案例   
    - rag-evaluation                # 多模型评估，模型响应结果，结合RAG的案例
    - rag-elasticsearch             # 基于ES的rag案例
mcp目录                             
    - client目录                        
        - mcp-stdio-client          # MCP的stdio客户端案例
        - mcp-webflux-client        # MCP的webflux客户端案例
        - mcp-nacos2-client         # MCP基于Nacos2.*实现分布式部署客户端案例
        - mcp-nacos3-client         # MCP基于Nacos3.*实现分布式部署客户端案例
    - server目录                     
        - mcp-stdio-server          # MCP的stdio服务端案例
        - mcp-webflux-server        # MCP的webflux服务端案例
        - mcp-nacos2-server         # MCP基于Nacos2.*实现分布式部署服务端案例
        - mcp-nacos3-server         # MCP基于Nacos3.*实现分布式部署服务端案例
        - mcp-dynamic-server(待补充) # MCP基于Nacos的动态restful服务端案例
        - mcp-swagger-server(待补充) # MCP基于Swagger的restful服务端案例       
observabilty                        # ObservationHandler下的client、model、tool、embedding的观测案例
graph目录  # 基于spring ai alibaba graph内核
    - simple                        # 最简单的graph案例
    - stream-node                   # 节点中AI模型的流式输出案例
    - human-node(待补充)             # 人类反馈中断、复原的案例
    - paraller-node                 # 多节点并行的案例
    - mcp-node                      # 配置指定mcp给指定node的案例
multi-agent目录
    - multipe-write（待补充）         # 多轮写作，基于人类反馈润色文章的案例
    - deep-research（待补充）         # 深度研究产出报告案例                           
```

微信推文系列免费：https://mp.weixin.qq.com/s/AacHsoJu4-qcscll07nW3A

文档地址：https://ik3te1knhq.feishu.cn/wiki/PdXhwljrZiDQ6mkmkrecBDm9nhh
- 文档中有系列快速上手+源码解读系列的详细解释（收费），获取文档权限
- Spring Ai Alibaba开源社区的Contributor可免费获取文档权限

<img src="docx/vx.png" style="width:120px">