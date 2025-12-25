
[[Traffic Control - Route Tables]]

|**Feature**|**Security Group (Instance Level)**|**Network ACL (Subnet Level)**|
|---|---|---|
|**Scope**|Operates at the **Task/Instance** level.|Operates at the **Subnet** level.|
|**State**|**Stateful**: If you allow an inbound request, the response is automatically allowed.|**Stateless**: You must explicitly allow both inbound and outbound traffic.|
|**Rules**|Supports **Allow** rules only.|Supports **Allow** and **Deny** rules.|
|**Order**|All rules are evaluated before traffic is allowed.|Rules are evaluated in chronological order (lowest number first).|