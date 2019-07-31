---
title: audioRoutingGroup リソースの種類
description: 音声ルーティンググループでは、複数の参加者の間のプライベートオーディオルートをマルチパーティの会話に格納します。 Source は参加者であり、受信者はマルチパーティの会話の他の参加者のサブセットです。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: db5f94f9ac500dfeb97c6eb787783e9f749ae507
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974277"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="b9e1a-104">audioRoutingGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b9e1a-104">audioRoutingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9e1a-105">音声ルーティンググループでは、複数の参加者の間のプライベートオーディオルートをマルチパーティの会話に格納します。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-105">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="b9e1a-106">Source は参加者であり、受信者はマルチパーティの会話の他の参加者のサブセットです。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-106">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="b9e1a-107">**注:**[ConfigureMixer](../api/participant-configuremixer.md)には、すべてのルートは含まれません。送信元と受信側の組み合わせにボリュームレベルを設定するための呼び出し全体に対して使用されます。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-107">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="b9e1a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b9e1a-108">Methods</span></span>

| <span data-ttu-id="b9e1a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b9e1a-109">Method</span></span>                                                  | <span data-ttu-id="b9e1a-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b9e1a-110">Return Type</span></span>                               | <span data-ttu-id="b9e1a-111">説明</span><span class="sxs-lookup"><span data-stu-id="b9e1a-111">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="b9e1a-112">AudioRoutingGroup を取得する</span><span class="sxs-lookup"><span data-stu-id="b9e1a-112">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="b9e1a-113">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b9e1a-113">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="b9e1a-114">AudioRoutingGroup オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-114">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="b9e1a-115">Update</span><span class="sxs-lookup"><span data-stu-id="b9e1a-115">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="b9e1a-116">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b9e1a-116">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="b9e1a-117">受信者の一覧を更新します。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-117">Update receivers list.</span></span>                       |
| [<span data-ttu-id="b9e1a-118">Delete</span><span class="sxs-lookup"><span data-stu-id="b9e1a-118">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="b9e1a-119">None</span><span class="sxs-lookup"><span data-stu-id="b9e1a-119">None</span></span>                                      | <span data-ttu-id="b9e1a-120">オーディオルーティンググループを削除します。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-120">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="b9e1a-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9e1a-121">Properties</span></span>

| <span data-ttu-id="b9e1a-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9e1a-122">Property</span></span>      | <span data-ttu-id="b9e1a-123">型</span><span class="sxs-lookup"><span data-stu-id="b9e1a-123">Type</span></span>              | <span data-ttu-id="b9e1a-124">説明</span><span class="sxs-lookup"><span data-stu-id="b9e1a-124">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="b9e1a-125">id</span><span class="sxs-lookup"><span data-stu-id="b9e1a-125">id</span></span>            | <span data-ttu-id="b9e1a-126">string</span><span class="sxs-lookup"><span data-stu-id="b9e1a-126">string</span></span>            | <span data-ttu-id="b9e1a-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-127">Read-only.</span></span> <span data-ttu-id="b9e1a-128">サーバーによって生成されます。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-128">Server generated.</span></span>                                         |
| <span data-ttu-id="b9e1a-129">配信</span><span class="sxs-lookup"><span data-stu-id="b9e1a-129">receivers</span></span>     | <span data-ttu-id="b9e1a-130">collection(string)</span><span class="sxs-lookup"><span data-stu-id="b9e1a-130">collection(string)</span></span> | <span data-ttu-id="b9e1a-131">受信側参加者 id のリスト。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-131">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="b9e1a-132">routingMode</span><span class="sxs-lookup"><span data-stu-id="b9e1a-132">routingMode</span></span>   | <span data-ttu-id="b9e1a-133">string</span><span class="sxs-lookup"><span data-stu-id="b9e1a-133">string</span></span>            | <span data-ttu-id="b9e1a-134">ルーティンググループモード。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-134">Routing group mode.</span></span>  <span data-ttu-id="b9e1a-135">可能な値は、`oneToOne`、`multicast` です。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-135">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="b9e1a-136">sources</span><span class="sxs-lookup"><span data-stu-id="b9e1a-136">sources</span></span>       | <span data-ttu-id="b9e1a-137">collection(string)</span><span class="sxs-lookup"><span data-stu-id="b9e1a-137">collection(string)</span></span> | <span data-ttu-id="b9e1a-138">ソース参加者 id のリスト。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-138">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="b9e1a-139">**注:** ルーティングモードは、送信元と受信者に対する制限を決定します。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-139">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="b9e1a-140">次のルーティンググループのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-140">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="b9e1a-141">`oneToOne`-ソースと受信者には、それぞれ1人の参加者のみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-141">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="b9e1a-142">`multicast`-ソースには1つの参加者がいますが、複数の受信者がいます。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-142">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="b9e1a-143">受信者の一覧が更新された可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-143">Receivers list may be updated.</span></span>

> <span data-ttu-id="b9e1a-144">**注:** 多数のオーディオルーティンググループ (参加者ごとに bot など) を作成する場合は、上位4台の主要なスピーカーのオーディオのみが転送されます。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-144">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="b9e1a-145">カスタマイズされたオーディオルーティンググループを使用している場合でも、メインミキサーでスピーカーの音量が十分でない場合は、このスピーカーと bot のみに専用のオーディオグループがある場合でも、そのユーザーは bot によって聞くことはできません。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-145">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="b9e1a-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b9e1a-146">Relationships</span></span>
<span data-ttu-id="b9e1a-147">なし</span><span class="sxs-lookup"><span data-stu-id="b9e1a-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9e1a-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b9e1a-148">JSON representation</span></span>

<span data-ttu-id="b9e1a-149">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b9e1a-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "string (identifier)",
  "receivers": [ "string" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "string" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
