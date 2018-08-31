# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="0b2e4-101">inferenceClassificationOverride リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0b2e4-101">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="0b2e4-102">特定の差出人からの着信メッセージを常時分類するためのユーザーのオーバーライドを表します。</span><span class="sxs-lookup"><span data-stu-id="0b2e4-102">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="0b2e4-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="0b2e4-103">Methods</span></span>

| <span data-ttu-id="0b2e4-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="0b2e4-104">Method</span></span>           | <span data-ttu-id="0b2e4-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0b2e4-105">Return Type</span></span>    |<span data-ttu-id="0b2e4-106">説明</span><span class="sxs-lookup"><span data-stu-id="0b2e4-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0b2e4-107">更新する</span><span class="sxs-lookup"><span data-stu-id="0b2e4-107">Update</span></span>](../api/inferenceclassificationoverride_update.md) | [<span data-ttu-id="0b2e4-108">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="0b2e4-108">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="0b2e4-109">指定のとおり、オーバーライドの **ClassifyAs** フィールドを変更します。</span><span class="sxs-lookup"><span data-stu-id="0b2e4-109">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="0b2e4-110">削除</span><span class="sxs-lookup"><span data-stu-id="0b2e4-110">Delete</span></span>](../api/inferenceclassificationoverride_delete.md) | <span data-ttu-id="0b2e4-111">なし</span><span class="sxs-lookup"><span data-stu-id="0b2e4-111">None</span></span> |<span data-ttu-id="0b2e4-112">その ID で指定されたオーバーライドを削除します。</span><span class="sxs-lookup"><span data-stu-id="0b2e4-112">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="0b2e4-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b2e4-113">Properties</span></span>
| <span data-ttu-id="0b2e4-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b2e4-114">Property</span></span>     | <span data-ttu-id="0b2e4-115">タイプ</span><span class="sxs-lookup"><span data-stu-id="0b2e4-115">Type</span></span>   |<span data-ttu-id="0b2e4-116">説明</span><span class="sxs-lookup"><span data-stu-id="0b2e4-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b2e4-117">classifyAs</span><span class="sxs-lookup"><span data-stu-id="0b2e4-117">classifyAs</span></span>|<span data-ttu-id="0b2e4-118">InferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="0b2e4-118">InferenceClassificationType</span></span>| <span data-ttu-id="0b2e4-119">特定の差出人からの着信メッセージを常時分類する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="0b2e4-119">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="0b2e4-120">可能な値は、`focused`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="0b2e4-120">The possible values are:</span></span>|
|<span data-ttu-id="0b2e4-121">ID</span><span class="sxs-lookup"><span data-stu-id="0b2e4-121">id</span></span>|<span data-ttu-id="0b2e4-122">文字列</span><span class="sxs-lookup"><span data-stu-id="0b2e4-122">string</span></span>| <span data-ttu-id="0b2e4-p102">オーバーライドの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0b2e4-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="0b2e4-125">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0b2e4-125">senderEmailAddress</span></span>|[<span data-ttu-id="0b2e4-126">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0b2e4-126">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="0b2e4-127">オーバーライドを作成する対象の差出人のメール アドレス情報。</span><span class="sxs-lookup"><span data-stu-id="0b2e4-127">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b2e4-128">関係</span><span class="sxs-lookup"><span data-stu-id="0b2e4-128">Relationships</span></span>
<span data-ttu-id="0b2e4-129">なし</span><span class="sxs-lookup"><span data-stu-id="0b2e4-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0b2e4-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0b2e4-130">JSON representation</span></span>

<span data-ttu-id="0b2e4-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0b2e4-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->