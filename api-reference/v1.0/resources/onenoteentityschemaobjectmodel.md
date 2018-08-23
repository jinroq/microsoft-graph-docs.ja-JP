# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="59590-101">onenoteEntitySchemaObjectModel リソース</span><span class="sxs-lookup"><span data-stu-id="59590-101">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="59590-102">OneNote エンティティの基本データ型です。</span><span class="sxs-lookup"><span data-stu-id="59590-102">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59590-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59590-103">JSON representation</span></span>

<span data-ttu-id="59590-104">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59590-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntitySchemaObjectModel"
}-->

```json
{
  "createdDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="59590-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59590-105">Properties</span></span>
| <span data-ttu-id="59590-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59590-106">Property</span></span>     | <span data-ttu-id="59590-107">型</span><span class="sxs-lookup"><span data-stu-id="59590-107">Type</span></span>   |<span data-ttu-id="59590-108">説明</span><span class="sxs-lookup"><span data-stu-id="59590-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59590-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59590-109">createdDateTime</span></span>|<span data-ttu-id="59590-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59590-110">DateTimeOffset</span></span>|<span data-ttu-id="59590-p101">ページが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="59590-p101">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->