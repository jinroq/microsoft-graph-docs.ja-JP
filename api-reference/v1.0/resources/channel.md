# <a name="channel-resource-type"></a><span data-ttu-id="6d0dc-101">チャネル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6d0dc-101">channel resource type</span></span>



<span data-ttu-id="6d0dc-102">チャネルは、[チーム](../resources/team.md)内でのメッセージのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-102">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="6d0dc-103">チャネルでは、トピックとチーム内での議論の論理的分離を表します。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-103">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="6d0dc-104">例としては、「金曜日チーム ランチ」のチャネルとチャネルの「アーキテクチャの説明」にあります。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-104">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="6d0dc-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="6d0dc-105">Methods</span></span>

| <span data-ttu-id="6d0dc-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="6d0dc-106">Method</span></span>       | <span data-ttu-id="6d0dc-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6d0dc-107">Return Type</span></span>  |<span data-ttu-id="6d0dc-108">説明</span><span class="sxs-lookup"><span data-stu-id="6d0dc-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6d0dc-109">チャネルのリスト</span><span class="sxs-lookup"><span data-stu-id="6d0dc-109">List channels</span></span>](../api/channel_list.md) | <span data-ttu-id="6d0dc-110">[チャネル](channel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6d0dc-110">[channel](channel.md) collection</span></span> | <span data-ttu-id="6d0dc-111">このチームでは、チャネルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-111">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="6d0dc-112">チャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-112">Create channel</span></span>](../api/channel_post.md) | [<span data-ttu-id="6d0dc-113">チャネル</span><span class="sxs-lookup"><span data-stu-id="6d0dc-113">channel</span></span>](channel.md) | <span data-ttu-id="6d0dc-114">表示名と説明を含めることで、新しいチャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-114">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="6d0dc-115">チャネルを取得します。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-115">Get channel</span></span>](../api/channel_get.md) | [<span data-ttu-id="6d0dc-116">チャネル</span><span class="sxs-lookup"><span data-stu-id="6d0dc-116">channel</span></span>](channel.md) | <span data-ttu-id="6d0dc-117">チャネルのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-117">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="6d0dc-118">チャネルを更新します。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-118">Update channel</span></span>](../api/channel_patch.md) | [<span data-ttu-id="6d0dc-119">チャネル</span><span class="sxs-lookup"><span data-stu-id="6d0dc-119">channel</span></span>](channel.md) | <span data-ttu-id="6d0dc-120">チャネルのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-120">Update properties of the channel.</span></span>|
|[<span data-ttu-id="6d0dc-121">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-121">Delete channel</span></span>](../api/channel_delete.md) | <span data-ttu-id="6d0dc-122">なし</span><span class="sxs-lookup"><span data-stu-id="6d0dc-122">None</span></span> | <span data-ttu-id="6d0dc-123">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-123">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="6d0dc-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d0dc-124">Properties</span></span>
| <span data-ttu-id="6d0dc-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d0dc-125">Property</span></span>     | <span data-ttu-id="6d0dc-126">型</span><span class="sxs-lookup"><span data-stu-id="6d0dc-126">Type</span></span>   |<span data-ttu-id="6d0dc-127">説明</span><span class="sxs-lookup"><span data-stu-id="6d0dc-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d0dc-128">説明</span><span class="sxs-lookup"><span data-stu-id="6d0dc-128">description</span></span>|<span data-ttu-id="6d0dc-129">文字列</span><span class="sxs-lookup"><span data-stu-id="6d0dc-129">String</span></span>|<span data-ttu-id="6d0dc-130">チャネルの省略可能な説明です。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-130">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="6d0dc-131">displayName</span><span class="sxs-lookup"><span data-stu-id="6d0dc-131">displayName</span></span>|<span data-ttu-id="6d0dc-132">文字列</span><span class="sxs-lookup"><span data-stu-id="6d0dc-132">String</span></span>|<span data-ttu-id="6d0dc-133">チャネルの名前は、マイクロソフトのチーム内のユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-133">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="6d0dc-134">id</span><span class="sxs-lookup"><span data-stu-id="6d0dc-134">id</span></span>|<span data-ttu-id="6d0dc-135">文字列</span><span class="sxs-lookup"><span data-stu-id="6d0dc-135">String</span></span>|<span data-ttu-id="6d0dc-136">チャネルの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-136">The channels's unique identifier.</span></span> <span data-ttu-id="6d0dc-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-137">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d0dc-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6d0dc-138">Relationships</span></span>
| <span data-ttu-id="6d0dc-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6d0dc-139">Relationship</span></span> | <span data-ttu-id="6d0dc-140">型</span><span class="sxs-lookup"><span data-stu-id="6d0dc-140">Type</span></span>   |<span data-ttu-id="6d0dc-141">説明</span><span class="sxs-lookup"><span data-stu-id="6d0dc-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d0dc-142">タブ</span><span class="sxs-lookup"><span data-stu-id="6d0dc-142">tabs</span></span>|<span data-ttu-id="6d0dc-143">[teamsTab](../resources/teamstab.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6d0dc-143">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="6d0dc-144">チャネル内のすべてのタブのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-144">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="6d0dc-145">ナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="6d0dc-145">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6d0dc-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6d0dc-146">JSON representation</span></span>

<span data-ttu-id="6d0dc-147">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6d0dc-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
