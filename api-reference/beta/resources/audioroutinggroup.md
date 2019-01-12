---
title: audioRoutingGroup リソースの種類
description: オーディオのルーティング グループでは、通話参加者の間にプライベート オーディオ ルートを格納します。 ソースは参加者自身で、受信者、通話の他の参加者のサブセットであります。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0e18a9beb660b9bae0c1bbe1034ec64790d369fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980189"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="a5bac-104">audioRoutingGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a5bac-104">audioRoutingGroup resource type</span></span>

> <span data-ttu-id="a5bac-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a5bac-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5bac-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5bac-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5bac-107">オーディオのルーティング グループでは、通話参加者の間にプライベート オーディオ ルートを格納します。</span><span class="sxs-lookup"><span data-stu-id="a5bac-107">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="a5bac-108">ソースは参加者自身で、受信者、通話の他の参加者のサブセットであります。</span><span class="sxs-lookup"><span data-stu-id="a5bac-108">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="a5bac-109">**注:**[ConfigureMixer](../api/participant-configuremixer.md)は、任意のルートを伴わないのすべての呼び出し元と受信者間の組み合わせのボリューム レベルを設定するためです。</span><span class="sxs-lookup"><span data-stu-id="a5bac-109">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="a5bac-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="a5bac-110">Methods</span></span>

| <span data-ttu-id="a5bac-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="a5bac-111">Method</span></span>                                                  | <span data-ttu-id="a5bac-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a5bac-112">Return Type</span></span>                               | <span data-ttu-id="a5bac-113">説明</span><span class="sxs-lookup"><span data-stu-id="a5bac-113">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="a5bac-114">AudioRoutingGroup を取得します。</span><span class="sxs-lookup"><span data-stu-id="a5bac-114">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="a5bac-115">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="a5bac-115">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="a5bac-116">AudioRoutingGroup オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5bac-116">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="a5bac-117">Update</span><span class="sxs-lookup"><span data-stu-id="a5bac-117">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="a5bac-118">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="a5bac-118">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="a5bac-119">受信者リストを更新します。</span><span class="sxs-lookup"><span data-stu-id="a5bac-119">Update receivers list.</span></span>                       |
| [<span data-ttu-id="a5bac-120">Delete</span><span class="sxs-lookup"><span data-stu-id="a5bac-120">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="a5bac-121">なし</span><span class="sxs-lookup"><span data-stu-id="a5bac-121">None</span></span>                                      | <span data-ttu-id="a5bac-122">オーディオのルーティング グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="a5bac-122">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="a5bac-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5bac-123">Properties</span></span>

| <span data-ttu-id="a5bac-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5bac-124">Property</span></span>      | <span data-ttu-id="a5bac-125">型</span><span class="sxs-lookup"><span data-stu-id="a5bac-125">Type</span></span>              | <span data-ttu-id="a5bac-126">説明</span><span class="sxs-lookup"><span data-stu-id="a5bac-126">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="a5bac-127">ID</span><span class="sxs-lookup"><span data-stu-id="a5bac-127">id</span></span>            | <span data-ttu-id="a5bac-128">String</span><span class="sxs-lookup"><span data-stu-id="a5bac-128">String</span></span>            | <span data-ttu-id="a5bac-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a5bac-129">Read-only.</span></span> <span data-ttu-id="a5bac-130">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="a5bac-130">Server generated.</span></span>                                         |
| <span data-ttu-id="a5bac-131">受信機</span><span class="sxs-lookup"><span data-stu-id="a5bac-131">receivers</span></span>     | <span data-ttu-id="a5bac-132">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a5bac-132">String Collection</span></span> | <span data-ttu-id="a5bac-133">参加者の id を受信する] ボックスの一覧です。</span><span class="sxs-lookup"><span data-stu-id="a5bac-133">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="a5bac-134">routingMode</span><span class="sxs-lookup"><span data-stu-id="a5bac-134">routingMode</span></span>   | <span data-ttu-id="a5bac-135">String</span><span class="sxs-lookup"><span data-stu-id="a5bac-135">String</span></span>            | <span data-ttu-id="a5bac-136">ルーティング グループのモードです。</span><span class="sxs-lookup"><span data-stu-id="a5bac-136">Routing group mode.</span></span>  <span data-ttu-id="a5bac-137">使用可能な値は、`oneToOne`、`multicast` です。</span><span class="sxs-lookup"><span data-stu-id="a5bac-137">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="a5bac-138">ソース</span><span class="sxs-lookup"><span data-stu-id="a5bac-138">sources</span></span>       | <span data-ttu-id="a5bac-139">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a5bac-139">String Collection</span></span> | <span data-ttu-id="a5bac-140">ソースの構成要素の id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="a5bac-140">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="a5bac-141">**注:** ルーティング モードでは、送信元と受信機の制限を決定します。</span><span class="sxs-lookup"><span data-stu-id="a5bac-141">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="a5bac-142">次のルーティング グループのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="a5bac-142">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="a5bac-143">`oneToOne`-ソースと受信機に 1 つだけの参加者がそれぞれが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a5bac-143">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="a5bac-144">`multicast`-ソース 1 人の参加者が複数の受信機があります。</span><span class="sxs-lookup"><span data-stu-id="a5bac-144">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="a5bac-145">受信者リストを更新する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a5bac-145">Receivers list may be updated.</span></span>

> <span data-ttu-id="a5bac-146">**注:** 多くのオーディオ ルーティング グループ (参加者ごとの bot など) を作成する場合は、4 最上位の優先度の高いスピーカーのオーディオのみが転送されます。</span><span class="sxs-lookup"><span data-stu-id="a5bac-146">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="a5bac-147">カスタマイズされたオーディオのルーティング グループを使用しても意味のスピーカーがおさまるように、メインのミキサーでない場合は、本人聞こえない bot でこのスピーカーと、bot のためだけのオーディオのプライベート グループがある場合でもします。</span><span class="sxs-lookup"><span data-stu-id="a5bac-147">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="a5bac-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a5bac-148">Relationships</span></span>
<span data-ttu-id="a5bac-149">なし</span><span class="sxs-lookup"><span data-stu-id="a5bac-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5bac-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a5bac-150">JSON representation</span></span>

<span data-ttu-id="a5bac-151">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a5bac-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "String (identifier)",
  "receivers": [ "String" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "String" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
