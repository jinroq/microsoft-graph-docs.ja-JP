# <a name="recipient-resource-type"></a><span data-ttu-id="e8c63-101">受信者リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8c63-101">recipient resource type</span></span>

<span data-ttu-id="e8c63-102">イベント、メッセージ、またはグループ投稿の送信側または受信側のユーザーに関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="e8c63-102">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="e8c63-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8c63-103">Properties</span></span>
| <span data-ttu-id="e8c63-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8c63-104">Property</span></span>     | <span data-ttu-id="e8c63-105">型</span><span class="sxs-lookup"><span data-stu-id="e8c63-105">Type</span></span>   |<span data-ttu-id="e8c63-106">説明</span><span class="sxs-lookup"><span data-stu-id="e8c63-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8c63-107">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e8c63-107">emailAddress</span></span>|[<span data-ttu-id="e8c63-108">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="e8c63-108">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="e8c63-109">受信者の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="e8c63-109">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8c63-110">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8c63-110">JSON representation</span></span>

<span data-ttu-id="e8c63-111">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e8c63-111">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->