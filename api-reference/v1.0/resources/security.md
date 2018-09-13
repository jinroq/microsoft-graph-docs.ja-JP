# <a name="security-resource-type"></a><span data-ttu-id="5bb93-101">セキュリティ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5bb93-101">security resource type</span></span>

<span data-ttu-id="5bb93-102">セキュリティ リソースは、セキュリティ オブジェクト モデルのエントリ ポイントです。</span><span class="sxs-lookup"><span data-stu-id="5bb93-102">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="5bb93-103">シングルトンのセキュリティ リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="5bb93-103">It returns a singleton security resource.</span></span> <span data-ttu-id="5bb93-104">使用可能なプロパティが含まれていません。</span><span class="sxs-lookup"><span data-stu-id="5bb93-104">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="5bb93-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="5bb93-105">Methods</span></span>

| <span data-ttu-id="5bb93-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="5bb93-106">Method</span></span>       | <span data-ttu-id="5bb93-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5bb93-107">Return Type</span></span> | <span data-ttu-id="5bb93-108">説明</span><span class="sxs-lookup"><span data-stu-id="5bb93-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5bb93-109">警告の一覧表示</span><span class="sxs-lookup"><span data-stu-id="5bb93-109">List alerts</span></span>](../api/alert_list.md) | <span data-ttu-id="5bb93-110">[アラート](alert.md) のコレクション</span><span class="sxs-lookup"><span data-stu-id="5bb93-110">[alert](alert.md) collection</span></span> | <span data-ttu-id="5bb93-111">警告オブジェクトのコレクションを取得。</span><span class="sxs-lookup"><span data-stu-id="5bb93-111">Get a licenseDetails object collection.</span></span> |
| [<span data-ttu-id="5bb93-112">アラートを取得</span><span class="sxs-lookup"><span data-stu-id="5bb93-112">get alerts</span></span>](../api/alert_get.md) | <span data-ttu-id="5bb93-113">[アラート](alert.md) のコレクション</span><span class="sxs-lookup"><span data-stu-id="5bb93-113">[alert](alert.md) collection</span></span> | <span data-ttu-id="5bb93-114">アラートオブジェクトを取得。</span><span class="sxs-lookup"><span data-stu-id="5bb93-114">Get a alert object.</span></span> |
| [<span data-ttu-id="5bb93-115">通知を更新</span><span class="sxs-lookup"><span data-stu-id="5bb93-115">Update alerts</span></span>](../api/alert_update.md) | <span data-ttu-id="5bb93-116">[アラート](alert.md) のコレクション</span><span class="sxs-lookup"><span data-stu-id="5bb93-116">[alert](alert.md) collection</span></span> | <span data-ttu-id="5bb93-117">アラートオブジェクトを取得。</span><span class="sxs-lookup"><span data-stu-id="5bb93-117">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5bb93-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5bb93-118">Properties</span></span>
<span data-ttu-id="5bb93-119">なし</span><span class="sxs-lookup"><span data-stu-id="5bb93-119">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5bb93-120">関係</span><span class="sxs-lookup"><span data-stu-id="5bb93-120">Relationships</span></span>
| <span data-ttu-id="5bb93-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5bb93-121">Relationship</span></span> | <span data-ttu-id="5bb93-122">型</span><span class="sxs-lookup"><span data-stu-id="5bb93-122">Type</span></span>        | <span data-ttu-id="5bb93-123">説明</span><span class="sxs-lookup"><span data-stu-id="5bb93-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5bb93-124">アラート</span><span class="sxs-lookup"><span data-stu-id="5bb93-124">alerts</span></span>|<span data-ttu-id="5bb93-125">[アラート](alert.md) のコレクション</span><span class="sxs-lookup"><span data-stu-id="5bb93-125">[alert](alert.md) collection</span></span>| <span data-ttu-id="5bb93-p102">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="5bb93-p102">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5bb93-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5bb93-128">JSON representation</span></span>
<span data-ttu-id="5bb93-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5bb93-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="5bb93-130">例</span><span class="sxs-lookup"><span data-stu-id="5bb93-130">Example</span></span>

<span data-ttu-id="5bb93-131">**プランナー** のリソースは、グラフのルートに使用できます。</span><span class="sxs-lookup"><span data-stu-id="5bb93-131">The **security** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->