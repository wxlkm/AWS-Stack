# AWS CloudFormation Stack Template

multi-tier-web-app-in-vpc.template
在VPC中部署一个多层应用

vpc-private.yaml
此 VPC 具有两个私有子网以及适用于 Amazon Simple Storage Service 和 Amazon DynamoDB 的 VPC 终端节点。您可以使用此模板为不需要 Internet 访问权限的函数创建 VPC。此配置支持与 AWS 软件开发包一起使用 Amazon S3 和 DynamoDB，以及通过本地网络连接访问相同 VPC 中的数据库资源。 

vpc-privatepublic.yaml
此 VPC 具有两个私有子网、VPC 终端节点、一个具有 NAT 网关的公有子网，以及一个 Internet 网关。来自私有子网中函数的 Internet 相关流量将通过路由表路由到 NAT 网关。 
