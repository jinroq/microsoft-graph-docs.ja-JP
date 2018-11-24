# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="d4575-101">teamGuestSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d4575-101">teamGuestSettings resource type</span></span>



<span data-ttu-id="d4575-102">来園者が作成、更新、または[チーム](team.md)内のチャンネルを削除するかどうかを構成するのに設定します。</span><span class="sxs-lookup"><span data-stu-id="d4575-102">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d4575-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4575-103">Properties</span></span>
| <span data-ttu-id="d4575-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4575-104">Property</span></span>     | <span data-ttu-id="d4575-105">型</span><span class="sxs-lookup"><span data-stu-id="d4575-105">Type</span></span>   |<span data-ttu-id="d4575-106">説明</span><span class="sxs-lookup"><span data-stu-id="d4575-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4575-107">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="d4575-107">allowCreateUpdateChannels</span></span>|<span data-ttu-id="d4575-108">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4575-108">Boolean</span></span>|<span data-ttu-id="d4575-109">True の場合、来園者のセットを追加したりチャンネルを更新する場合。</span><span class="sxs-lookup"><span data-stu-id="d4575-109">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="d4575-110">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="d4575-110">allowDeleteChannels</span></span>|<span data-ttu-id="d4575-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4575-111">Boolean</span></span>|<span data-ttu-id="d4575-112">場合は true を指定すると、来園者に設定するには、チャンネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="d4575-112">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4575-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d4575-113">JSON representation</span></span>

<span data-ttu-id="d4575-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d4575-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
