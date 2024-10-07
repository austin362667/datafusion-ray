<!---
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

# TPC-H

## Running Benchmarks

Data and queries must be available on all nodes of the Ray cluster.

```shell
 RAY_ADDRESS='http://ray-cluster-ip-address:8265'  ray job submit --working-dir `pwd` -- python3 tpcbench.py --benchmark tpch --data /path/to/data --queries /path/to/tpch/queries --concurrency 4
```