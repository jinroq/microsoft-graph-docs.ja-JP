# <a name="messageruleactions-resource-type"></a><span data-ttu-id="bde1e-101">messageRuleActions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bde1e-101">messageRuleActions resource type</span></span>


<span data-ttu-id="bde1e-102">ルールに使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="bde1e-102">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="bde1e-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bde1e-103">Properties</span></span>
| <span data-ttu-id="bde1e-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bde1e-104">Property</span></span>     | <span data-ttu-id="bde1e-105">タイプ</span><span class="sxs-lookup"><span data-stu-id="bde1e-105">Type</span></span>   |<span data-ttu-id="bde1e-106">説明</span><span class="sxs-lookup"><span data-stu-id="bde1e-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bde1e-107">assignCategories</span><span class="sxs-lookup"><span data-stu-id="bde1e-107">assignCategories</span></span> | <span data-ttu-id="bde1e-108">String コレクション</span><span class="sxs-lookup"><span data-stu-id="bde1e-108">String collection</span></span> | <span data-ttu-id="bde1e-109">メッセージに割り当てられるカテゴリの一覧です。</span><span class="sxs-lookup"><span data-stu-id="bde1e-109">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="bde1e-110">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="bde1e-110">copyToFolder</span></span> | <span data-ttu-id="bde1e-111">文字列</span><span class="sxs-lookup"><span data-stu-id="bde1e-111">String</span></span> | <span data-ttu-id="bde1e-112">メッセージのコピー先のフォルダーの ID です。</span><span class="sxs-lookup"><span data-stu-id="bde1e-112">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="bde1e-113">削除</span><span class="sxs-lookup"><span data-stu-id="bde1e-113">delete</span></span> | <span data-ttu-id="bde1e-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="bde1e-114">Boolean</span></span> | <span data-ttu-id="bde1e-115">削除済みアイテム フォルダーにメッセージを移動する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bde1e-115">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="bde1e-116">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="bde1e-116">forwardAsAttachmentTo</span></span> | <span data-ttu-id="bde1e-117">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bde1e-117">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="bde1e-118">添付ファイルとしてメッセージを転送する受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="bde1e-118">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="bde1e-119">forwardTo</span><span class="sxs-lookup"><span data-stu-id="bde1e-119">forwardTo</span></span> | <span data-ttu-id="bde1e-120">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bde1e-120">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="bde1e-121">メッセージを転送する受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="bde1e-121">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="bde1e-122">markAsRead</span><span class="sxs-lookup"><span data-stu-id="bde1e-122">markAsRead</span></span> | <span data-ttu-id="bde1e-123">ブール値</span><span class="sxs-lookup"><span data-stu-id="bde1e-123">Boolean</span></span> | <span data-ttu-id="bde1e-124">メッセージを開封済みにする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bde1e-124">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="bde1e-125">markImportance</span><span class="sxs-lookup"><span data-stu-id="bde1e-125">markImportance</span></span> | <span data-ttu-id="bde1e-126">重要性</span><span class="sxs-lookup"><span data-stu-id="bde1e-126">importance</span></span> | <span data-ttu-id="bde1e-127">メッセージの重要性: `low`、`normal`、`high` を設定します。</span><span class="sxs-lookup"><span data-stu-id="bde1e-127">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="bde1e-128">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="bde1e-128">moveToFolder</span></span> |  <span data-ttu-id="bde1e-129">文字列</span><span class="sxs-lookup"><span data-stu-id="bde1e-129">String</span></span>| <span data-ttu-id="bde1e-130">メッセージ移動先のフォルダーの ID です。</span><span class="sxs-lookup"><span data-stu-id="bde1e-130">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="bde1e-131">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="bde1e-131">permanentDelete</span></span> | <span data-ttu-id="bde1e-132">ブール値</span><span class="sxs-lookup"><span data-stu-id="bde1e-132">Boolean</span></span> | <span data-ttu-id="bde1e-133">メッセージを完全に削除し、削除済みアイテム フォルダーにメッセージを保存しないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bde1e-133">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="bde1e-134">redirectTo</span><span class="sxs-lookup"><span data-stu-id="bde1e-134">redirectTo</span></span> | <span data-ttu-id="bde1e-135">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bde1e-135">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="bde1e-136">メッセージのリダイレクト先の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="bde1e-136">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="bde1e-137">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="bde1e-137">stopProcessingRules</span></span> | <span data-ttu-id="bde1e-138">ブール値</span><span class="sxs-lookup"><span data-stu-id="bde1e-138">Boolean</span></span> | <span data-ttu-id="bde1e-139">後続のルールを評価する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bde1e-139">Indicates whether subsequent rules should be evaluated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bde1e-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bde1e-140">JSON representation</span></span>
<span data-ttu-id="bde1e-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bde1e-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->