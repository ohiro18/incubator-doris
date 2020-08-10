---
{
    "title": "Show Runtime Info Action",
    "language": "zh-CN"
}
---

<!-- 
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
-->

# Show Runtime Info Action

## Request

`GET /api/show_runtime_info`

## Description

用于获取 FE JVM 的 Runtime 信息
    
## Path parameters

无

## Query parameters

无

## Request body

无

## Response

```
{
	"msg": "success",
	"code": 0,
	"data": {
		"free_mem": "855642056",
		"total_mem": "1037959168",
		"thread_cnt": "98",
		"max_mem": "1037959168"
	},
	"count": 0
}
```
    
## Examples

1. 回去当前 FE 节点的 JVM 信息

    ```
    GET /api/show_runtime_info
    
    Response:
    {
    	"msg": "success",
    	"code": 0,
    	"data": {
    		"free_mem": "855642056",
    		"total_mem": "1037959168",
    		"thread_cnt": "98",
    		"max_mem": "1037959168"
    	},
    	"count": 0
    }
    ```