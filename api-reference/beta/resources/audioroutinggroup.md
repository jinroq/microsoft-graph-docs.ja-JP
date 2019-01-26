---
title: audioRoutingGroup リソースの種類
description: オーディオのルーティング グループでは、通話参加者の間にプライベート オーディオ ルートを格納します。 ソースは参加者自身で、受信者、通話の他の参加者のサブセットであります。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fb1303e2a6f9e269faf5767093d418cdd0980463
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573019"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="9a49c-104">audioRoutingGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9a49c-104">audioRoutingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a49c-105">オーディオのルーティング グループでは、通話参加者の間にプライベート オーディオ ルートを格納します。</span><span class="sxs-lookup"><span data-stu-id="9a49c-105">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="9a49c-106">ソースは参加者自身で、受信者、通話の他の参加者のサブセットであります。</span><span class="sxs-lookup"><span data-stu-id="9a49c-106">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="9a49c-107">**注:**[ConfigureMixer](../api/participant-configuremixer.md)は、任意のルートを伴わないのすべての呼び出し元と受信者間の組み合わせのボリューム レベルを設定するためです。</span><span class="sxs-lookup"><span data-stu-id="9a49c-107">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="9a49c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9a49c-108">Methods</span></span>

| <span data-ttu-id="9a49c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="9a49c-109">Method</span></span>                                                  | <span data-ttu-id="9a49c-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9a49c-110">Return Type</span></span>                               | <span data-ttu-id="9a49c-111">説明</span><span class="sxs-lookup"><span data-stu-id="9a49c-111">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="9a49c-112">AudioRoutingGroup を取得します。</span><span class="sxs-lookup"><span data-stu-id="9a49c-112">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="9a49c-113">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="9a49c-113">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="9a49c-114">AudioRoutingGroup オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a49c-114">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="9a49c-115">Update</span><span class="sxs-lookup"><span data-stu-id="9a49c-115">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="9a49c-116">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="9a49c-116">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="9a49c-117">受信者リストを更新します。</span><span class="sxs-lookup"><span data-stu-id="9a49c-117">Update receivers list.</span></span>                       |
| [<span data-ttu-id="9a49c-118">Delete</span><span class="sxs-lookup"><span data-stu-id="9a49c-118">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="9a49c-119">なし</span><span class="sxs-lookup"><span data-stu-id="9a49c-119">None</span></span>                                      | <span data-ttu-id="9a49c-120">オーディオのルーティング グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="9a49c-120">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="9a49c-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a49c-121">Properties</span></span>

| <span data-ttu-id="9a49c-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a49c-122">Property</span></span>      | <span data-ttu-id="9a49c-123">型</span><span class="sxs-lookup"><span data-stu-id="9a49c-123">Type</span></span>              | <span data-ttu-id="9a49c-124">説明</span><span class="sxs-lookup"><span data-stu-id="9a49c-124">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="9a49c-125">id</span><span class="sxs-lookup"><span data-stu-id="9a49c-125">id</span></span>            | <span data-ttu-id="9a49c-126">String</span><span class="sxs-lookup"><span data-stu-id="9a49c-126">String</span></span>            | <span data-ttu-id="9a49c-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9a49c-127">Read-only.</span></span> <span data-ttu-id="9a49c-128">サーバーを生成します。</span><span class="sxs-lookup"><span data-stu-id="9a49c-128">Server generated.</span></span>                                         |
| <span data-ttu-id="9a49c-129">受信機</span><span class="sxs-lookup"><span data-stu-id="9a49c-129">receivers</span></span>     | <span data-ttu-id="9a49c-130">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9a49c-130">String Collection</span></span> | <span data-ttu-id="9a49c-131">参加者の id を受信する] ボックスの一覧です。</span><span class="sxs-lookup"><span data-stu-id="9a49c-131">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="9a49c-132">routingMode</span><span class="sxs-lookup"><span data-stu-id="9a49c-132">routingMode</span></span>   | <span data-ttu-id="9a49c-133">String</span><span class="sxs-lookup"><span data-stu-id="9a49c-133">String</span></span>            | <span data-ttu-id="9a49c-134">ルーティング グループのモードです。</span><span class="sxs-lookup"><span data-stu-id="9a49c-134">Routing group mode.</span></span>  <span data-ttu-id="9a49c-135">使用可能な値は、`oneToOne`、`multicast` です。</span><span class="sxs-lookup"><span data-stu-id="9a49c-135">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="9a49c-136">ソース</span><span class="sxs-lookup"><span data-stu-id="9a49c-136">sources</span></span>       | <span data-ttu-id="9a49c-137">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9a49c-137">String Collection</span></span> | <span data-ttu-id="9a49c-138">ソースの構成要素の id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="9a49c-138">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="9a49c-139">**注:** ルーティング モードでは、送信元と受信機の制限を決定します。</span><span class="sxs-lookup"><span data-stu-id="9a49c-139">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="9a49c-140">次のルーティング グループのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9a49c-140">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="9a49c-141">`oneToOne`-ソースと受信機に 1 つだけの参加者がそれぞれが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9a49c-141">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="9a49c-142">`multicast`-ソース 1 人の参加者が複数の受信機があります。</span><span class="sxs-lookup"><span data-stu-id="9a49c-142">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="9a49c-143">受信者リストを更新する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="9a49c-143">Receivers list may be updated.</span></span>

> <span data-ttu-id="9a49c-144">**注:** 多くのオーディオ ルーティング グループ (参加者ごとの bot など) を作成する場合は、4 最上位の優先度の高いスピーカーのオーディオのみが転送されます。</span><span class="sxs-lookup"><span data-stu-id="9a49c-144">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="9a49c-145">カスタマイズされたオーディオのルーティング グループを使用しても意味のスピーカーがおさまるように、メインのミキサーでない場合は、本人聞こえない bot でこのスピーカーと、bot のためだけのオーディオのプライベート グループがある場合でもします。</span><span class="sxs-lookup"><span data-stu-id="9a49c-145">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="9a49c-146">関係</span><span class="sxs-lookup"><span data-stu-id="9a49c-146">Relationships</span></span>
<span data-ttu-id="9a49c-147">なし</span><span class="sxs-lookup"><span data-stu-id="9a49c-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a49c-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9a49c-148">JSON representation</span></span>

<span data-ttu-id="9a49c-149">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a49c-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "String (identifier)",
  "receivers": [ "Guid" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "Guid" ]
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
  "suppressions": [
    "Error: /api-reference/beta/resources/audioroutinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
