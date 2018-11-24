# <a name="operationerror-resource-type"></a><span data-ttu-id="95c6b-101">operationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95c6b-101">operationError resource type</span></span>



<span data-ttu-id="95c6b-102">[TeamsAsyncOperation](teamsasyncoperation.md)で発生したエラーをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="95c6b-102">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="95c6b-103">operationError プロパティ</span><span class="sxs-lookup"><span data-stu-id="95c6b-103">operationError Properties</span></span>
| <span data-ttu-id="95c6b-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95c6b-104">Property</span></span>     | <span data-ttu-id="95c6b-105">型</span><span class="sxs-lookup"><span data-stu-id="95c6b-105">Type</span></span>   |<span data-ttu-id="95c6b-106">説明</span><span class="sxs-lookup"><span data-stu-id="95c6b-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95c6b-107">code</span><span class="sxs-lookup"><span data-stu-id="95c6b-107">code</span></span>|<span data-ttu-id="95c6b-108">文字列 (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="95c6b-108">string (readonly)</span></span>|<span data-ttu-id="95c6b-109">操作のエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="95c6b-109">Operation error code.</span></span>|
|<span data-ttu-id="95c6b-110">message</span><span class="sxs-lookup"><span data-stu-id="95c6b-110">message</span></span>|<span data-ttu-id="95c6b-111">文字列 (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="95c6b-111">string (readonly)</span></span>|<span data-ttu-id="95c6b-112">エラー メッセージを操作します。</span><span class="sxs-lookup"><span data-stu-id="95c6b-112">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95c6b-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95c6b-113">JSON representation</span></span>

<span data-ttu-id="95c6b-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="95c6b-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
