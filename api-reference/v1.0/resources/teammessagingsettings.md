# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="65d7a-101">teamMessagingSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65d7a-101">teamMessagingSettings resource type</span></span>



<span data-ttu-id="65d7a-102">メッセージングを構成する設定は、[チーム](team.md)内の参照。</span><span class="sxs-lookup"><span data-stu-id="65d7a-102">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="65d7a-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65d7a-103">Properties</span></span>
| <span data-ttu-id="65d7a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65d7a-104">Property</span></span>     | <span data-ttu-id="65d7a-105">型</span><span class="sxs-lookup"><span data-stu-id="65d7a-105">Type</span></span>   |<span data-ttu-id="65d7a-106">説明</span><span class="sxs-lookup"><span data-stu-id="65d7a-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65d7a-107">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="65d7a-107">allowUserEditMessages</span></span>|<span data-ttu-id="65d7a-108">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d7a-108">Boolean</span></span>|<span data-ttu-id="65d7a-109">場合 true の場合、ユーザーに設定するには、自分のメッセージを編集できます。</span><span class="sxs-lookup"><span data-stu-id="65d7a-109">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="65d7a-110">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="65d7a-110">allowUserDeleteMessages</span></span>|<span data-ttu-id="65d7a-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d7a-111">Boolean</span></span>|<span data-ttu-id="65d7a-112">場合は true の場合、ユーザーに設定するには、そのメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="65d7a-112">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="65d7a-113">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="65d7a-113">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="65d7a-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d7a-114">Boolean</span></span>|<span data-ttu-id="65d7a-115">場合は true の場合、所有者に設定するには、任意のメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="65d7a-115">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="65d7a-116">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="65d7a-116">allowTeamMentions</span></span>|<span data-ttu-id="65d7a-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d7a-117">Boolean</span></span>|<span data-ttu-id="65d7a-118">場合、参照投稿を許可する @team を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="65d7a-118">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="65d7a-119">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="65d7a-119">allowChannelMentions</span></span>|<span data-ttu-id="65d7a-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="65d7a-120">Boolean</span></span>|<span data-ttu-id="65d7a-121">場合、参照投稿を許可する @channel を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="65d7a-121">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65d7a-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65d7a-122">JSON representation</span></span>

<span data-ttu-id="65d7a-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="65d7a-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
