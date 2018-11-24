# <a name="teamstab-resource-type"></a><span data-ttu-id="a0308-101">teamsTab リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a0308-101">teamsTab resource type</span></span>



<span data-ttu-id="a0308-102">[] タブ](../resources/teamstab.md)では、teamsTab を[チーム](team.md)内での[チャネル](channel.md)(接続) を固定しました。</span><span class="sxs-lookup"><span data-stu-id="a0308-102">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="a0308-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="a0308-103">Methods</span></span>

| <span data-ttu-id="a0308-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="a0308-104">Method</span></span>       | <span data-ttu-id="a0308-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a0308-105">Return Type</span></span>  |<span data-ttu-id="a0308-106">説明</span><span class="sxs-lookup"><span data-stu-id="a0308-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0308-107">[一覧] タブ](../api/teamstab_list.md)</span><span class="sxs-lookup"><span data-stu-id="a0308-107">[List tabs](../api/teamstab_list.md)</span></span> | [<span data-ttu-id="a0308-108">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0308-108">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a0308-109">リスト タブは、チャンネルに固定します。</span><span class="sxs-lookup"><span data-stu-id="a0308-109">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="a0308-110">タブを取得します。</span><span class="sxs-lookup"><span data-stu-id="a0308-110">Get tab</span></span>](../api/teamstab_get.md) | [<span data-ttu-id="a0308-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0308-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a0308-112">チャンネルに固定されているタブを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a0308-112">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="a0308-113">タブを追加します。</span><span class="sxs-lookup"><span data-stu-id="a0308-113">Add tab</span></span>](../api/teamstab_add.md) | [<span data-ttu-id="a0308-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0308-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a0308-115">(ピン) を追加するチャンネルをタブします。</span><span class="sxs-lookup"><span data-stu-id="a0308-115">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="a0308-116">タブを削除します。</span><span class="sxs-lookup"><span data-stu-id="a0308-116">Remove tab</span></span>](../api/teamstab_delete.md) | <span data-ttu-id="a0308-117">なし</span><span class="sxs-lookup"><span data-stu-id="a0308-117">None</span></span> | <span data-ttu-id="a0308-118">削除 (固定解除) チャネルからタブします。</span><span class="sxs-lookup"><span data-stu-id="a0308-118">Removes (unpins) a tab from a channel.</span></span>|
|<span data-ttu-id="a0308-119">[[更新] タブ](../api/teamstab_update.md)</span><span class="sxs-lookup"><span data-stu-id="a0308-119">[Update tab](../api/teamstab_update.md)</span></span> | [<span data-ttu-id="a0308-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0308-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a0308-121">タブのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a0308-121">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="a0308-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0308-122">Properties</span></span>

|<span data-ttu-id="a0308-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0308-123">Property</span></span>|<span data-ttu-id="a0308-124">型</span><span class="sxs-lookup"><span data-stu-id="a0308-124">Type</span></span>|<span data-ttu-id="a0308-125">説明</span><span class="sxs-lookup"><span data-stu-id="a0308-125">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="a0308-126">ID</span><span class="sxs-lookup"><span data-stu-id="a0308-126">id</span></span>              |   <span data-ttu-id="a0308-127">文字列</span><span class="sxs-lookup"><span data-stu-id="a0308-127">string</span></span>                  |  <span data-ttu-id="a0308-128">チャネル タブ読み取りのみの特定のインスタンスを一意に識別する識別子です。</span><span class="sxs-lookup"><span data-stu-id="a0308-128">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="a0308-129">displayName</span><span class="sxs-lookup"><span data-stu-id="a0308-129">displayName</span></span>            |   <span data-ttu-id="a0308-130">string</span><span class="sxs-lookup"><span data-stu-id="a0308-130">string</span></span>                  |  <span data-ttu-id="a0308-131">タブの名前です。</span><span class="sxs-lookup"><span data-stu-id="a0308-131">Name of the tab.</span></span>     |
|  <span data-ttu-id="a0308-132">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="a0308-132">sortOrderIndex</span></span>  |   <span data-ttu-id="a0308-133">int</span><span class="sxs-lookup"><span data-stu-id="a0308-133">int</span></span>                     |  <span data-ttu-id="a0308-134">タブの並べ替え順序のインデックス</span><span class="sxs-lookup"><span data-stu-id="a0308-134">Index of the order used for sorting tabs</span></span>     |
|  <span data-ttu-id="a0308-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="a0308-135">webUrl</span></span>          |   <span data-ttu-id="a0308-136">文字列</span><span class="sxs-lookup"><span data-stu-id="a0308-136">string</span></span>                  |  <span data-ttu-id="a0308-137">タブのインスタンスの高度なリンクの url です。</span><span class="sxs-lookup"><span data-stu-id="a0308-137">Deep link url of the tab instance.</span></span> <span data-ttu-id="a0308-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a0308-138">Read only.</span></span>     |
|  <span data-ttu-id="a0308-139">configuration</span><span class="sxs-lookup"><span data-stu-id="a0308-139">configuration</span></span>        |   [<span data-ttu-id="a0308-140">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0308-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="a0308-141">タブに適用するカスタム設定のコンテナーです。タブでは、このプロパティが 1 回だけが構成されていると見なされます。</span><span class="sxs-lookup"><span data-stu-id="a0308-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="a0308-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a0308-142">Relationships</span></span>

| <span data-ttu-id="a0308-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a0308-143">Relationship</span></span> | <span data-ttu-id="a0308-144">型</span><span class="sxs-lookup"><span data-stu-id="a0308-144">Type</span></span>   | <span data-ttu-id="a0308-145">説明</span><span class="sxs-lookup"><span data-stu-id="a0308-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a0308-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a0308-146">teamsApp</span></span>|[<span data-ttu-id="a0308-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a0308-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="a0308-148">タブにリンクされているアプリケーションです。タブを作成した後は、これを変更できません。</span><span class="sxs-lookup"><span data-stu-id="a0308-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a0308-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a0308-149">JSON representation</span></span>

<span data-ttu-id="a0308-150">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a0308-150">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="a0308-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="a0308-151">See also</span></span>

[<span data-ttu-id="a0308-152">組み込みタブのタイプを設定します。</span><span class="sxs-lookup"><span data-stu-id="a0308-152">Configuring the built-in tab types</span></span>](../../../concepts/teams-configuring-builtin-tabs.md)
