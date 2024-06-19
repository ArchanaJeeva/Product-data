**Evaluation Warning : The document was created with Spire.Presentation for Python** 

**IBM Fusion HCI ![](Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.001.jpeg)**

The easiest way to run **OpenShift**  applications and **watsonx** 

Configuration guide ![](Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.002.png)

Bill Stoddard – Program Director and Product Manager, IBM Fusion HCI May 1, 2024 

**IBM Internal and Business Partner Use only** 

**Evaluation Warning : The document was created with Spire.Presentation for Python**

IBM Fusion HCI and watsonx™ are better together

Integrated OpenShift application platform optimized for **watsonx**

Hyper-converged systems with NVMe  **FUSION BENEFITS ![](Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.003.png)Compute/storage nodes ![](Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.004.png)![](Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.005.png)**

32 or 64 core 

256/512/1024/2048 GB memory ✓ Rapid deployment

- Deploy Fusion HCI application platform in under a week

NVIDIA L40S GPU • Reduce project risk and uncertainty with tested, optimized system **GPU nodes** • Accelerate time to value![](Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.006.png)

Up to 16x NVIDIA L40S 

GPUs ✓ Highest performance

Dedicated 100 GbE storage network •• Bare-metal OpenShift eliminates hypervisor overheadHyper-converged systems with fast NVMe local drives

**High speed switches** • S3 endpoints backed by scale-out parallel file system![](Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.007.png)

100 GbE storage network

25 GbE pod network ✓ Accelerate queries from remote object stores

- Speed up queries from remote object stores by up to **90X**
- S3 object
- Azure Blob

Optional S3 external storage

**IBM Storage Ceph** ✓ Start small, upgrade in-field ![](Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.008.png)96/144/192/240 TB raw • Add compute

HDD for data

SSD for metadata • Add local storage

- Add remote query acceleration

Optional remote object query accelerator • Add remote object storage

**AFM nodes** ✓ Single Support

Accelerate remote queries![](Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.009.png)

S3 object stores One call for full stack support Azure Blob

Why watsonx on Fusion HCI are better together 

Differentiators

**Evaluation Warning : The document was created with Spire.Presentation for Python**

**Reduce TCO by up to 83% (1)**

- Fusion HCI delivers performance and cost efficiency of bare-metal OpenShift 
- … combined with the operational simplicity of hyper-convergence
- Efficient 4+2p erasure coding maximizes availability of local NVMe storage
- Eliminate hypervisor cost overhead

**Highest performance (2)**

- P03 6-node configurations start at 700K IOPS and 80 GB/s throughput
  - P11 14-node configurations max out at 1.6M IOPS and 180 GB/s
  - IOPS and throughput scale linearly with addition of storage nodes
- S3 endpoints backed by parallel file system is much faster than SAN storage
- Eliminate hypervisor performance overhead

**High reliability and resiliency under load**

- Dedicated and redundant 100 GbE storage pod network
- Dedicated and redundant 25 GbE application pod network

**Reduced risk of project failures**

- Turnkey appliance-like deployment
- Engineered solution reduces risk of improper infrastructure design and missed performance objectives
- Integrated solution is fully tested and validated with watsonx
1) Blinded TCO study of Fusion HCI with a U.S. nationally recognized banking and insurance company
1) Using Global Data Platform storage provider.  P03 and P11 refer to specific Fusion HCI t-shirt sizes  See charts later in this deck for details

**Flexible non-disruptive scaling – start small and grow** 

- Single racks can support **watsonx.data** data lakes from 59 TB to 699 TB
- Cluster up to 3 racks to expand capacity
- Add remote query acceleration for highest performance

**Expand watsonx.data data lake capacity to petabytes**

- Use Ceph ready-nodes to grow safe, private **watsonx.data** data lates
- Cost effective data lakes that can grow to multiple petabytes

**Accelerate watsonx.data queries to remote object stores**

- Combined with **watsonx.data** query optimization, Fusion HCI accelerates queries to any S3 compliant object stores.
- Up to 90x boost in query performance

**Fusion HCI Query Accelerator – How it works**

- **Leverages local NVMe storage as cache for remote data**
- Transparently mirror remote data residing on multiple S3 or Azure Blob
- Use policies to configure cache operations – fetch data on demand, pre- fetch data, set cache size, set expiration/eviction policies
- Cached data is available to all compute nodes through S3 endpoints 
- S3 endpoints backed by the Fusion high performance scale-out parallel file system

**IBM Internal and Business Partner Use only**

**Evaluation Warning : The document was created with Spire.Presentation for Python**

Fusion HCI “E” series bucket sizes ![ref1]

Fusion HCI “E” series features **32 core storage rich servers** each with 512 GB of memory and  **IBM Fusion** HCI two (2) 3.84 TB drives per server.



<table><tr><th colspan="2">Fusion HCI</th><th colspan="1">E03</th><th colspan="1">E04</th><th colspan="1">E05</th><th colspan="1">E06</th><th colspan="1">E07</th><th colspan="1">E08</th><th colspan="1">E09</th><th colspan="1">E10</th><th colspan="1">E11</th></tr>
<tr><td colspan="1" rowspan="8" valign="top"><p><b>Fusion</b></p><p>HCI</p></td><td colspan="1">Total vCPU (1)</td><td colspan="1">96</td><td colspan="1">128</td><td colspan="1">160</td><td colspan="1">192</td><td colspan="1">224</td><td colspan="1">256</td><td colspan="1">288</td><td colspan="1">320</td><td colspan="1">352</td></tr>
<tr><td colspan="1"><p><b>Available vCPU (1)</b></p><p>(SMT=2)</p></td><td colspan="1"><b>60</b> (120)</td><td colspan="1"><b>80</b> (160)</td><td colspan="1"><b>100</b> (200)</td><td colspan="1"><b>120</b> (240)</td><td colspan="1"><b>140</b> (280)</td><td colspan="1"><b>160</b> (320)</td><td colspan="1"><b>180</b> (360)</td><td colspan="1"><b>200</b> (400)</td><td colspan="1"><b>220</b> (440)</td></tr>
<tr><td colspan="1">Available memory(2) (GB)</td><td colspan="1">1296</td><td colspan="1">1,728</td><td colspan="1">2160</td><td colspan="1">2,592</td><td colspan="1">3024</td><td colspan="1">3,456</td><td colspan="1">3888</td><td colspan="1">4,320</td><td colspan="1">4752</td></tr>
<tr><td colspan="1" valign="top"><p>Usable NVMe (3)</p><p>(TiB)</p></td><td colspan="1" valign="top">~27 TiB</td><td colspan="1" valign="top">~31 TiB</td><td colspan="1" valign="top">~36 TiB</td><td colspan="1" valign="top">~40 TiB</td><td colspan="1" valign="top">~45 TiB</td><td colspan="1" valign="top">~49 TiB</td><td colspan="1" valign="top">~54 TiB</td><td colspan="1" valign="top">~59 TiB</td><td colspan="1" valign="top">~63 TiB</td></tr>
<tr><td colspan="1" valign="top"><p>NVMe drives</p><p>(3.84 TB)</p></td><td colspan="1" valign="top">12</td><td colspan="1" valign="top">14</td><td colspan="1" valign="top">16</td><td colspan="1" valign="top">18</td><td colspan="1" valign="top">20</td><td colspan="1" valign="top">22</td><td colspan="1" valign="top">24</td><td colspan="1" valign="top">26</td><td colspan="1" valign="top">28</td></tr>
<tr><td colspan="1">Worker nodes</td><td colspan="1">3</td><td colspan="1">4</td><td colspan="1">5</td><td colspan="1">6</td><td colspan="1">7</td><td colspan="1">8</td><td colspan="1">9</td><td colspan="1">10</td><td colspan="1">11</td></tr>
<tr><td colspan="1">Control nodes</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td></tr>
<tr><td colspan="1"><p>Fusion Software</p><p>VPC</p></td><td colspan="1">96</td><td colspan="1">128</td><td colspan="1">160</td><td colspan="1">192</td><td colspan="1">224</td><td colspan="1">256</td><td colspan="1">288</td><td colspan="1">320</td><td colspan="1">352</td></tr>
</table>

**Expansion options / add-ons: Notes: ![ref2]**

- GPU servers with from 1 to 8 NVIDIA L40S GPUs per server The “E” series Fusion HCI are the lowest in absolute cost, but  
- AFM query acceleration nodes for watsonx.data they have limited maximum configuration size compared to the  
- Additional NVMe drives, up to 10 per server “P” series.   
- 3.84 or 7.68 TB drives 
- 32 core compute only servers 
- 64 core compute only servers 
1) Fusion HCI supports hyper-threading. The first row is vCPU at SMT=1 (no hyper-threading). The second row is vCPU with SMT=2 (with hyper-threading). **IBM Internal and** 
1) These “E” series include 256 GB memory upgrades on each server. You can reduce cost by deleting the memory upgrade. **Business Partner Use only**
1) Usable storage with 3.84 TB drives using the Scale ECE / Global Data Platform storage provider

(3) Usable storage with 3.84 TB drives using the Scale ECE / Global Data Platform storage provider
**Evaluation Warning : The document was created with Spire.Presentation for Python**

Fusion HCI “P” series bucket sizes![](Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.012.png)![ref2]![ref1]

Fusion HCI “P” series features **64 core storage rich servers** each with 2048 GB of memory and two (2) 3.84 TB drives per server.



<table><tr><th colspan="2">Fusion HCI</th><th colspan="1">P03</th><th colspan="1">P04</th><th colspan="1">P05</th><th colspan="1">P06</th><th colspan="1">P07</th><th colspan="1">P08</th><th colspan="1">P09</th><th colspan="1">P10</th><th colspan="1">P11</th></tr>
<tr><td colspan="1" rowspan="8" valign="top"><b>Fusion</b> HCI</td><td colspan="1">Total vCPU (1)</td><td colspan="1">192</td><td colspan="1">256</td><td colspan="1">320</td><td colspan="1">384</td><td colspan="1">448</td><td colspan="1">512</td><td colspan="1">576</td><td colspan="1">640</td><td colspan="1">704</td></tr>
<tr><td colspan="1"><p><b>Available vCPU (1)</b></p><p>(SMT=2)</p></td><td colspan="1"><b>156</b> (312)</td><td colspan="1"><b>208</b> (416)</td><td colspan="1"><b>260</b> (520)</td><td colspan="1"><b>312</b> (624)</td><td colspan="1"><b>364</b> (728)</td><td colspan="1"><b>416</b> (832)</td><td colspan="1"><b>468</b> (936)</td><td colspan="1"><b>520</b> (1040)</td><td colspan="1"><b>572</b> (1144)</td></tr>
<tr><td colspan="1"><p>Available memory </p><p>(2) (GB)</p></td><td colspan="1">5,904</td><td colspan="1">7,872</td><td colspan="1">9,840</td><td colspan="1">11,808</td><td colspan="1">13,776</td><td colspan="1">15,744</td><td colspan="1">17,712</td><td colspan="1">19,680</td><td colspan="1">21,648</td></tr>
<tr><td colspan="1" valign="top"><p>Usable NVMe (3)</p><p>(TiB)</p></td><td colspan="1" valign="top">~27 TiB</td><td colspan="1" valign="top">~31 TiB</td><td colspan="1" valign="top">~36 TiB</td><td colspan="1" valign="top">~40 TiB</td><td colspan="1" valign="top">~45 TiB</td><td colspan="1" valign="top">~49 TiB</td><td colspan="1" valign="top">~54 TiB</td><td colspan="1" valign="top">~59 TiB</td><td colspan="1" valign="top">~63 TiB</td></tr>
<tr><td colspan="1" valign="top"><p>NVMe drives</p><p>(3.84 TB)</p></td><td colspan="1" valign="top">12</td><td colspan="1" valign="top">14</td><td colspan="1" valign="top">16</td><td colspan="1" valign="top">18</td><td colspan="1" valign="top">20</td><td colspan="1" valign="top">22</td><td colspan="1" valign="top">24</td><td colspan="1" valign="top">26</td><td colspan="1" valign="top">28</td></tr>
<tr><td colspan="1">Worker nodes</td><td colspan="1">3</td><td colspan="1">4</td><td colspan="1">5</td><td colspan="1">6</td><td colspan="1">7</td><td colspan="1">8</td><td colspan="1">9</td><td colspan="1">10</td><td colspan="1">11</td></tr>
<tr><td colspan="1">Control nodes</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td></tr>
<tr><td colspan="1"><p>Fusion software </p><p>VPC</p></td><td colspan="1" valign="top">192</td><td colspan="1" valign="top">256</td><td colspan="1" valign="top">320</td><td colspan="1" valign="top">384</td><td colspan="1" valign="top">448</td><td colspan="1" valign="top">512</td><td colspan="1" valign="top">576</td><td colspan="1" valign="top">640</td><td colspan="1" valign="top">704</td></tr>
</table>

**Expansion options / add-ons: Notes:**

- GPU servers with from 1 to 8 NVIDIA L40S GPUs per server The “P” series Fusion HCI are optimized for watsonx.data 
- AFM query acceleration nodes for watsonx.data performance.  Lots of memory, lots of cores, and they can be 
- Additional NVMe drives, up to 10 per server expanded to bigger sizes than the “E” series.  The “P” series are more cost effective in terms of cost per vCPU for large or multiple 
- 3.84 or 7.68 TB drives workloads.
- 32 core compute only servers
- 64 core compute only servers
1) Fusion HCI supports hyper-threading. The first row is vCPU at SMT=1 (no hyper-threading). The second row is vCPU with SMT=2 (with hyper-threading).
1) These “P” series include 1024 GB memory upgrades on each server. You can reduce cost by deleting the memory upgrade.

**IBM Fusion** HCI

(3) Usable storage with 3.84 TB drives using the Scale ECE / Global Data Platform storage provider
**Evaluation Warning : The document was created with Spire.Presentation for Python** 

Fusion HCI configuration and expansion options ![ref1]![](Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.013.png)

**IBM Fusion** HCI

All Fusion HCI configurations can be upgraded in the field. Clients can start small  and add compute and storage as their workloads grow ![ref2]



||||
| :- | :- | :- |
|Fusion HCI expansion options||Description|
|<p>Two (2) AFM query acceleration </p><p>nodes (4)</p>|•|**Compute servers to automatically load data from remote S3 and Azure Blob object stores into Fusion HCI local storage cache. Fusion software VPC not required for these nodes. (useful for watsonx.data)**|
|NVIDIA L40S GPU Servers|•|**Each 9155-G03 servers has 48 vCPU of x86 cores and holds from 1 to 8 NVIDIA L40S GPUs. Each G03 requires 48 VPC of Fusion software**|
|3\.84 TB NVMe drives|• •|**E04 and P04 can be expanded up to 70 NVMe drives in increments of 14 drives P08 can be expanded  up to 110 NVMe drives in increments of 22 drives**|
|7\.68 TB NVMe drives|•|**Replace 3.84 TB drives with 7.68 TB drives to increase max capacity.**|
|32 core compute servers|•|**Add 26 usable vCPU for other workloads.  Requires 32 VPC of Fusion software**|
|64 core compute servers|•|**Add 52 usable vCPU for other workloads. Requires 64 VPC of Fusion software**|

(1) See speaker notes 


**Evaluation Warning : The document was created with Spire.Presentation for Python**

Fusion HCI watsonx.ai use cases and model coverage ![](Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.014.png)Fusion HCI Foundation Model Coverage

|**Models**|**Size**|**Fusion HCI Type**|**L40S (48GB)**|
| - | - | - | - |
|flan-t5-xl-3b|3B|Small|1 GPU|
|Flan-t5-xxl-11b|11B|Small|1 GPU|
|Flan-ul2-20b|20B|Medium|2 GPU\*|
|Gpt-neox-20b|20B|Medium|2 GPU\*|
|Granite-13b-chat-v2|13B|Small|1 GPU|
|Granite-13b-chat-v1|13B|Small|1 GPU|
|Granite-13b-instruct-v2|13B|Small|1 GPU|
|Granite-13b-instructv1|13B|Small|1 GPU|
|Llama2-chat-13b|13B|Small|1 GPU|
|Llama-2-70b-chat|70B|Large|4 GPU\*|
|Mpt-7b-instruct2|7B|Small|1 GPU|
|Mt0-xxl-13b|13B|Small|1 GPU|
|Starcoder-15.5b|15\.5B|Small|1 GPU|
|Mixtral-8x7b-instruct|7B|Small|1 GPU|
|Elyza-Japanese-llama2-7b-instruct|7B|Small|1 GPU|

Use Cases and Capabilities

- Model serving/inferencing performance optimized and tuned on Fusion HCI

•

Prompt Lab to experiment with foundation models and build prompts for various use cases and tasks

- Foundation Model Library with IBM and open-source models

•

NLP Use Cases summarization, generation, classification, extraction, and Q&A / retrieval augmented generation (RAG)

- Jupyter Notebook recipes for NLP use cases

•

Tuning Studio to tune your foundation models with labeled data

\* L40S does not support NVLink reducing model sharding performance. H100, which does support Nvlink, is close on Fusion HCI horizon.

More about Fusion HCI configurations

**Fusion HCI memory**

Memory is a cost-effective way to boost watsonx.data performance. The “E” and “P” series Fusion HCI configurations feature upgraded memory.  The “E” series servers have been upgraded with 256 GB of additional memory, for a total of 512 GB per server.  The “P” series servers have been upgraded with 1024 GB of memory, for a total of 204 GB per server. 

**Query acceleration upgrade - Active File Management (AFM)** 

Fusion HCI with the Global Data Platform provider supports caching remote object store data in the local NVMe based file system.  The cache is dynamic in that it can fetch or pre-fetch data, age out old entries, and it can be configured for either uni-directional / read only or bi-directional / read-write.  Use of AFM query acceleration requires that Fusion HCI be upgraded with a pair of AFM servers (9155-C10 servers).  Adding more NVMe drives to storage servers is also advisable to enable more of the remote data to be cached locally.

**Storage capacity upgrade**

Each server in the Fusion HCI “E” and “P” series has two (2) NVMe drives per server.  You can upgrade these servers to have up to 10 drives per server.  Furthermore, you have two choices of drive sizes, either 7.68 or 3.84 TB.  Note: Mixing drive sizes in a cluster is not permitted. 

**Add compute without adding additional storage**

The “E” and “P” series features storage-rich servers. That is, all servers have NVMe drives.  You can also add 32 core or 64 core compute only servers to any of the “E” and “P” series configurations.   This might be desirable when you have enough storage and only need to add additional compute capacity.  

**The benefit of using storage-rich servers is data i/o performance**

Fusion HCI with the Scale ECE provider presents applications with a scale-out parallel file system. In practice, this means that each storage-rich server can support roughly 115K IOPS and 12 GB/s throughput. For example, the E03 configuration has a total of 6 storage-rich servers, thus an E03 can support up 690K IOPS and 72 GB/s throughput. IOPS and throughput increase linearly with each additional storage-rich server. 

**OpenShift subscriptions**

Fusion HCI does not include subscriptions to OpenShift. OpenShift subscriptions can be brought to Fusion HCI through the workload (eg restricted subscriptions included with Cloud Paks), or purchased separately from Red Hat, IBM, or Red Hat business partners. Fusion HCI qualifies for socket-pair bare- metal subscriptions. Core-pair subscriptions will be needed for virtualized clusters hosted with Red Hat Hosted Control Planes on Fusion HCI.

**Evaluation Warning : The document was created with Spire.Presentation for Python**

“E” series configurations example pricing

Example pricing with 1 year of support. Configurations include two (2) 3.84 TB NVMe drives and 512 GB of memory per server.



<table><tr><th colspan="2">Fusion HCI</th><th colspan="1">E03</th><th colspan="1">E05</th><th colspan="1">E07</th><th colspan="1">E09</th><th colspan="1">E11</th></tr>
<tr><td colspan="1" rowspan="9"><p>Fusion HCI</p><p>Hardware</p></td><td colspan="1"><p>Control nodes</p><p>9155-C10</p></td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td></tr>
<tr><td colspan="1"><p>Worker nodes</p><p>9155-C10</p></td><td colspan="1">3</td><td colspan="1">5</td><td colspan="1">7</td><td colspan="1">9</td><td colspan="1">11</td></tr>
<tr><td colspan="1"><p>Available vCPU (1)</p><p>(SMT=1)(1)</p></td><td colspan="1"><p>120 </p><p>(60)</p></td><td colspan="1"><p>200</p><p>(100)</p></td><td colspan="1"><p>280</p><p>(140)</p></td><td colspan="1"><p>360</p><p>(180)</p></td><td colspan="1"><p>440</p><p>(220)</p></td></tr>
<tr><td colspan="1">Available Memory (GB)</td><td colspan="1">1296</td><td colspan="1">2160</td><td colspan="1">3024</td><td colspan="1">3888</td><td colspan="1">4752</td></tr>
<tr><td colspan="1"><p>NVMe drives</p><p>(3.84 TB)</p></td><td colspan="1">12</td><td colspan="1">16</td><td colspan="1">20</td><td colspan="1">24</td><td colspan="1">28</td></tr>
<tr><td colspan="1">Available NVMe (TiB)</td><td colspan="1">~27 TiB</td><td colspan="1">~36 TiB</td><td colspan="1">~45 TiB</td><td colspan="1">~54 TiB</td><td colspan="1">~63 TiB</td></tr>
<tr><td colspan="1">List</td><td colspan="1">$512.1K</td><td colspan="1">$634K</td><td colspan="1">$755K</td><td colspan="1">$876.5K</td><td colspan="1">$998K</td></tr>
<tr><td colspan="1">Discount</td><td colspan="1">73%</td><td colspan="1">73%</td><td colspan="1">73%</td><td colspan="1">73%</td><td colspan="1">73%</td></tr>
<tr><td colspan="1"><b>Net price + shipping</b></td><td colspan="1"><b>$143.7K</b></td><td colspan="1"><b>$177K</b></td><td colspan="1"><b>$210.3K</b></td><td colspan="1"><b>$243.6K</b></td><td colspan="1"><b>$276.9</b></td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><p>Fusion Software</p><p>5771-PP7</p></td><td colspan="1">License VPC</td><td colspan="1">96</td><td colspan="1">160</td><td colspan="1">224</td><td colspan="1">288</td><td colspan="1">352</td></tr>
<tr><td colspan="1">List</td><td colspan="1">$196.8K</td><td colspan="1">$328</td><td colspan="1">$459.2</td><td colspan="1">$590.4K</td><td colspan="1">$721.6K</td></tr>
<tr><td colspan="1">Discount</td><td colspan="1">75%</td><td colspan="1">75%</td><td colspan="1">75%</td><td colspan="1">75%</td><td colspan="1">75%</td></tr>
<tr><td colspan="1"><b>Net price</b></td><td colspan="1"><b>$49.2K</b></td><td colspan="1"><b>$82K</b></td><td colspan="1"><b>$114.8K</b></td><td colspan="1"><b>$147.6K</b></td><td colspan="1"><b>$180.4K</b></td></tr>
<tr><td colspan="1" valign="bottom">Premium Support</td><td colspan="1" valign="top"><p>1-year Premium</p><p>with TAM </p></td><td colspan="1" valign="top"><b>$18.8K</b></td><td colspan="1" valign="top"><b>$25.3K</b></td><td colspan="1" valign="top"><b>$31.9K</b></td><td colspan="1" valign="top"><b>$38.4K</b></td><td colspan="1" valign="top"><b>$45K</b></td></tr>
<tr><td colspan="1"><b>TOTAL</b></td><td colspan="1"></td><td colspan="1"><b>$211.6K</b></td><td colspan="1"><b>$284.3K</b></td><td colspan="1"><b>$357K</b></td><td colspan="1"><b>$429.7K</b></td><td colspan="1"><b>$502.3K</b></td></tr>
</table>



1) Fusion HCI servers support hyper-threading at SMT=2.  Available vCPU is presented for SMT=2 and SMT=1 in parenthesis 
1) Technology Expert Labs Fusion HCI install service is required except in US, Canada, and Japan. 2-week engagement is $27.4K. Includes one additional on-site upgrade service in the year

**IBM Fusion** HCI

![ref2]![ref3]![ref1]

**IBM Internal and Business Partner Use only**

“P” series configurations example pricing

Example pricing with 1 year of support. Configurations include two (2) 3.84 TB NVMe drives and 2048 GB of memory per server.



<table><tr><th colspan="2">Fusion HCI</th><th colspan="1">P03</th><th colspan="1">P05</th><th colspan="1">P07</th><th colspan="1">P09</th><th colspan="1">P11</th></tr>
<tr><td colspan="1" rowspan="9"><p>Fusion HCI</p><p>Hardware</p></td><td colspan="1"><p>Control nodes</p><p>9155-C10</p></td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td><td colspan="1">3</td></tr>
<tr><td colspan="1"><p>Worker nodes</p><p>9155-C14</p></td><td colspan="1">3</td><td colspan="1">5</td><td colspan="1">7</td><td colspan="1">9</td><td colspan="1">11</td></tr>
<tr><td colspan="1"><p>Available vCPU (1)</p><p>(SMT=1)(1)</p></td><td colspan="1"><p>312</p><p>(156)</p></td><td colspan="1"><p>520</p><p>(260)</p></td><td colspan="1"><p>728</p><p>(364)</p></td><td colspan="1"><p>936</p><p>(468)</p></td><td colspan="1"><p>1144</p><p>(572)</p></td></tr>
<tr><td colspan="1">Available Memory (GB)</td><td colspan="1">1296</td><td colspan="1">2160</td><td colspan="1">3024</td><td colspan="1">3888</td><td colspan="1">4752</td></tr>
<tr><td colspan="1"><p>NVMe drives</p><p>(3.84 TB)</p></td><td colspan="1">12</td><td colspan="1">16</td><td colspan="1">20</td><td colspan="1">24</td><td colspan="1">28</td></tr>
<tr><td colspan="1">Available NVMe (TiB)</td><td colspan="1">~27 TiB</td><td colspan="1">~36 TiB</td><td colspan="1">~45 TiB</td><td colspan="1">~54 TiB</td><td colspan="1">~63 TiB</td></tr>
<tr><td colspan="1">List</td><td colspan="1">$672.2K</td><td colspan="1">$900.5K</td><td colspan="1">$1128.7K</td><td colspan="1">$1357K</td><td colspan="1">$1585.3</td></tr>
<tr><td colspan="1">Discount</td><td colspan="1">73%</td><td colspan="1">73%</td><td colspan="1">73%</td><td colspan="1">73%</td><td colspan="1">73%</td></tr>
<tr><td colspan="1"><b>Net price + shipping</b></td><td colspan="1"><b>$186.9K</b></td><td colspan="1"><b>$249.1K</b></td><td colspan="1"><b>$311.2</b></td><td colspan="1"><b>$373.4</b></td><td colspan="1"><b>$435.5</b></td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><p>Fusion Software</p><p>5771-PP7</p></td><td colspan="1">License VPC</td><td colspan="1">192</td><td colspan="1">320</td><td colspan="1">448</td><td colspan="1">576</td><td colspan="1">704</td></tr>
<tr><td colspan="1">List</td><td colspan="1">$393.6K</td><td colspan="1">$656K</td><td colspan="1">$918.4K</td><td colspan="1">$1180.8K</td><td colspan="1">$1443.2K</td></tr>
<tr><td colspan="1">Discount</td><td colspan="1">75%</td><td colspan="1">75%</td><td colspan="1">75%</td><td colspan="1">75%</td><td colspan="1">75%</td></tr>
<tr><td colspan="1"><b>Net price</b></td><td colspan="1"><b>$98.4K</b></td><td colspan="1"><b>$164K</b></td><td colspan="1"><b>$229.6</b></td><td colspan="1"><b>$295.2K</b></td><td colspan="1"><b>$360.8K</b></td></tr>
<tr><td colspan="1" valign="bottom">Premium Support</td><td colspan="1" valign="top"><p>1-year Premium</p><p>with TAM </p></td><td colspan="1" valign="top"><b>$28K</b></td><td colspan="1" valign="top"><b>$40.7</b></td><td colspan="1" valign="top"><b>$53.5</b></td><td colspan="1" valign="top"><b>$66.2</b></td><td colspan="1" valign="top"><b>$78.9</b></td></tr>
<tr><td colspan="1"><b>TOTAL</b></td><td colspan="1"></td><td colspan="1"><b>$313.3</b></td><td colspan="1"><b>$453.8K</b></td><td colspan="1"><b>$594.2K</b></td><td colspan="1"><b>$734.7</b></td><td colspan="1"><b>$875.2</b></td></tr>
</table>



1) Fusion HCI servers support hyper-threading at SMT=2.  Available vCPU is presented for SMT=2 and SMT=1 in parenthesis 
1) Technology Expert Labs Fusion HCI install service is required except in US, Canada, and Japan. 2-week engagement is $27.4K. Includes one additional on-site upgrade service in the year

**IBM Fusion** HCI

![ref2]![ref3]![ref1]

**IBM Internal and Business Partner Use only**

[ref1]: Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.010.png
[ref2]: Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.011.png
[ref3]: Aspose.Words.c59346b0-e5d2-40c0-94d0-b9d4af99c217.015.png
