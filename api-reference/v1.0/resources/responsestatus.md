# <a name="responsestatus-resource-type"></a><span data-ttu-id="83f79-101">responseStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="83f79-101">responseStatus resource type</span></span>

<span data-ttu-id="83f79-102">会議出席依頼の応答状態です。</span><span class="sxs-lookup"><span data-stu-id="83f79-102">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="83f79-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83f79-103">Properties</span></span>

| <span data-ttu-id="83f79-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83f79-104">Property</span></span> | <span data-ttu-id="83f79-105">タイプ</span><span class="sxs-lookup"><span data-stu-id="83f79-105">Type</span></span>           | <span data-ttu-id="83f79-106">説明</span><span class="sxs-lookup"><span data-stu-id="83f79-106">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="83f79-107">response</span><span class="sxs-lookup"><span data-stu-id="83f79-107">response</span></span> | <span data-ttu-id="83f79-108">ResponseType</span><span class="sxs-lookup"><span data-stu-id="83f79-108">ResponseType</span></span>   | <span data-ttu-id="83f79-109">応答の種類。</span><span class="sxs-lookup"><span data-stu-id="83f79-109">The response type.</span></span> <span data-ttu-id="83f79-110">指定できる値: `None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded`。</span><span class="sxs-lookup"><span data-stu-id="83f79-110">The possible values are `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`, , , , , , or .</span></span>
| <span data-ttu-id="83f79-111">time</span><span class="sxs-lookup"><span data-stu-id="83f79-111">time</span></span>     | <span data-ttu-id="83f79-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83f79-112">DateTimeOffset</span></span> | <span data-ttu-id="83f79-p102">応答が返された日時。ISO 8601 形式を使って表され、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="83f79-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="83f79-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="83f79-116">JSON representation</span></span>

<span data-ttu-id="83f79-117">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="83f79-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
