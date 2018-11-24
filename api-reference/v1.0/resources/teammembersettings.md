# <a name="teammembersettings-resource-type"></a><span data-ttu-id="6f65c-101">teamMemberSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6f65c-101">teamMemberSettings resource type</span></span>



<span data-ttu-id="6f65c-102">など、メンバーが特定のアクションを実行するかどうかを構成する設定は、チャネルを作成し、[チーム](team.md)にボットを追加します。</span><span class="sxs-lookup"><span data-stu-id="6f65c-102">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6f65c-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f65c-103">Properties</span></span>
| <span data-ttu-id="6f65c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f65c-104">Property</span></span>     | <span data-ttu-id="6f65c-105">型</span><span class="sxs-lookup"><span data-stu-id="6f65c-105">Type</span></span>   |<span data-ttu-id="6f65c-106">説明</span><span class="sxs-lookup"><span data-stu-id="6f65c-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f65c-107">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="6f65c-107">allowCreateUpdateChannels</span></span>|<span data-ttu-id="6f65c-108">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f65c-108">Boolean</span></span>|<span data-ttu-id="6f65c-109">True の場合、メンバー セットを追加したりチャンネルを更新する場合。</span><span class="sxs-lookup"><span data-stu-id="6f65c-109">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="6f65c-110">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="6f65c-110">allowDeleteChannels</span></span>|<span data-ttu-id="6f65c-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f65c-111">Boolean</span></span>|<span data-ttu-id="6f65c-112">場合は true の場合、メンバーに設定するには、チャンネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="6f65c-112">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="6f65c-113">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="6f65c-113">allowAddRemoveApps</span></span>|<span data-ttu-id="6f65c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f65c-114">Boolean</span></span>|<span data-ttu-id="6f65c-115">場合は true の場合、メンバー セットは、追加し、アプリケーションを削除できます。</span><span class="sxs-lookup"><span data-stu-id="6f65c-115">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="6f65c-116">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="6f65c-116">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="6f65c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f65c-117">Boolean</span></span>|<span data-ttu-id="6f65c-118">場合は true の場合、メンバー セットを追加、更新、およびタブを削除します。</span><span class="sxs-lookup"><span data-stu-id="6f65c-118">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="6f65c-119">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="6f65c-119">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="6f65c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f65c-120">Boolean</span></span>|<span data-ttu-id="6f65c-121">場合は true の場合、メンバー セットを追加、更新、およびコネクタを削除します。</span><span class="sxs-lookup"><span data-stu-id="6f65c-121">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f65c-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6f65c-122">JSON representation</span></span>

<span data-ttu-id="6f65c-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6f65c-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
