# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="29531-101">onenoteEntityHierarchyModel リソース</span><span class="sxs-lookup"><span data-stu-id="29531-101">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="29531-102">これは、OneNote エンティティの基本データ型です。</span><span class="sxs-lookup"><span data-stu-id="29531-102">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="29531-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29531-103">JSON representation</span></span>

<span data-ttu-id="29531-104">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29531-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityHierarchyModel"
}-->

```json
{
  "displayName": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="29531-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29531-105">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="29531-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29531-106">Properties</span></span>
| <span data-ttu-id="29531-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29531-107">Property</span></span>     | <span data-ttu-id="29531-108">タイプ</span><span class="sxs-lookup"><span data-stu-id="29531-108">Type</span></span>   |<span data-ttu-id="29531-109">説明</span><span class="sxs-lookup"><span data-stu-id="29531-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29531-110">displayName</span><span class="sxs-lookup"><span data-stu-id="29531-110">displayName</span></span>|<span data-ttu-id="29531-111">文字列</span><span class="sxs-lookup"><span data-stu-id="29531-111">String</span></span>|<span data-ttu-id="29531-112">ノートブックの名前。</span><span class="sxs-lookup"><span data-stu-id="29531-112">The name of the notebook.</span></span>|
|<span data-ttu-id="29531-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="29531-113">createdBy</span></span>|[<span data-ttu-id="29531-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="29531-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="29531-p101">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="29531-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="29531-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="29531-117">lastModifiedBy</span></span>|[<span data-ttu-id="29531-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="29531-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="29531-p102">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="29531-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="29531-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29531-121">lastModifiedDateTime</span></span>|<span data-ttu-id="29531-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29531-122">DateTimeOffset</span></span>|<span data-ttu-id="29531-p103">ノートブックが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="29531-p103">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->