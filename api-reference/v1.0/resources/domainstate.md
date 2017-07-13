<span data-ttu-id="48421-p102">非同期操作の種類。値は、*ForceDelete* または *Verification* のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="48421-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> | 非同期操作の種類。値は、*ForceDelete* または *Verification* のいずれかです。 |
| <span data-ttu-id="48421-115">status</span><span class="sxs-lookup"><span data-stu-id="48421-115">status</span></span> | <span data-ttu-id="48421-116">String</span><span class="sxs-lookup"><span data-stu-id="48421-116">String</span></span> | <span data-ttu-id="48421-117">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="48421-117">Current status of the operation.</span></span> <br> <span data-ttu-id="48421-118">*Scheduled* - 操作はスケジュールされていますが、開始されていません。</span><span class="sxs-lookup"><span data-stu-id="48421-118">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="48421-119">*InProgress* - タスクが開始され、実行中です。</span><span class="sxs-lookup"><span data-stu-id="48421-119">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="48421-120">*Failed* - 操作が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="48421-120">*Failed* - Operation has failed.</span></span> |

## <span data-ttu-id="48421-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48421-121">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="48421-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="48421-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->