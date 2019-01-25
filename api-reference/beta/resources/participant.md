---
title: 参加者のリソースの種類
description: 参加者のタイプです。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f49526824b2b6c4eb4a5065f05ab4c765d299faa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508147"
---
# <a name="participant-resource-type"></a><span data-ttu-id="299e5-103">参加者のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="299e5-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="299e5-104">参加者のタイプです。</span><span class="sxs-lookup"><span data-stu-id="299e5-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="299e5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="299e5-105">Methods</span></span>

| <span data-ttu-id="299e5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="299e5-106">Method</span></span>                                                          | <span data-ttu-id="299e5-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="299e5-107">Return Type</span></span>                              | <span data-ttu-id="299e5-108">説明</span><span class="sxs-lookup"><span data-stu-id="299e5-108">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="299e5-109">構成要素を取得します。</span><span class="sxs-lookup"><span data-stu-id="299e5-109">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="299e5-110">参加者</span><span class="sxs-lookup"><span data-stu-id="299e5-110">participant</span></span>](participant.md)            | <span data-ttu-id="299e5-111">**構成要素**オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="299e5-111">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="299e5-112">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="299e5-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="299e5-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="299e5-113">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="299e5-114">参加者のオーディオ ミキサーを構成します。</span><span class="sxs-lookup"><span data-stu-id="299e5-114">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="299e5-115">招待</span><span class="sxs-lookup"><span data-stu-id="299e5-115">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="299e5-116">commsOperation</span><span class="sxs-lookup"><span data-stu-id="299e5-116">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="299e5-117">通話に参加者を招待します。</span><span class="sxs-lookup"><span data-stu-id="299e5-117">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="299e5-118">参加者のミュート</span><span class="sxs-lookup"><span data-stu-id="299e5-118">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="299e5-119">commsOperation</span><span class="sxs-lookup"><span data-stu-id="299e5-119">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="299e5-120">呼び出し内の参加者をミュートします。</span><span class="sxs-lookup"><span data-stu-id="299e5-120">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="299e5-121">参加者全員をミュートします。</span><span class="sxs-lookup"><span data-stu-id="299e5-121">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="299e5-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="299e5-122">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="299e5-123">会議のすべての参加者をミュートします。</span><span class="sxs-lookup"><span data-stu-id="299e5-123">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="299e5-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="299e5-124">Properties</span></span>

| <span data-ttu-id="299e5-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="299e5-125">Property</span></span>             | <span data-ttu-id="299e5-126">型</span><span class="sxs-lookup"><span data-stu-id="299e5-126">Type</span></span>                                     | <span data-ttu-id="299e5-127">説明</span><span class="sxs-lookup"><span data-stu-id="299e5-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="299e5-128">id</span><span class="sxs-lookup"><span data-stu-id="299e5-128">id</span></span>                   | <span data-ttu-id="299e5-129">String</span><span class="sxs-lookup"><span data-stu-id="299e5-129">String</span></span>                                   | <span data-ttu-id="299e5-130">参加者の id です。</span><span class="sxs-lookup"><span data-stu-id="299e5-130">The participant id.</span></span>                                          |
| <span data-ttu-id="299e5-131">Info</span><span class="sxs-lookup"><span data-stu-id="299e5-131">info</span></span>                 | [<span data-ttu-id="299e5-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="299e5-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="299e5-133">参加者の参加者です。</span><span class="sxs-lookup"><span data-stu-id="299e5-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="299e5-134">isInLobby</span><span class="sxs-lookup"><span data-stu-id="299e5-134">isInLobby</span></span>            | <span data-ttu-id="299e5-135">boolean</span><span class="sxs-lookup"><span data-stu-id="299e5-135">boolean</span></span>                                  | <span data-ttu-id="299e5-136">参加者がロビーに入っている場合は true。</span><span class="sxs-lookup"><span data-stu-id="299e5-136">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="299e5-137">isMuted</span><span class="sxs-lookup"><span data-stu-id="299e5-137">isMuted</span></span>              | <span data-ttu-id="299e5-138">boolean</span><span class="sxs-lookup"><span data-stu-id="299e5-138">boolean</span></span>                                  | <span data-ttu-id="299e5-139">参加者がミュートされている場合は true (クライアントまたはサーバーがミュートになって)</span><span class="sxs-lookup"><span data-stu-id="299e5-139">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="299e5-140">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="299e5-140">mediaStreams</span></span>         | <span data-ttu-id="299e5-141">[mediaStream](mediastream.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="299e5-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="299e5-142">メディア ストリームのリスト。</span><span class="sxs-lookup"><span data-stu-id="299e5-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="299e5-143">metadata</span><span class="sxs-lookup"><span data-stu-id="299e5-143">metadata</span></span>             | <span data-ttu-id="299e5-144">String</span><span class="sxs-lookup"><span data-stu-id="299e5-144">String</span></span>                                   | <span data-ttu-id="299e5-145">名簿にある参加者が提供するデータの blob</span><span class="sxs-lookup"><span data-stu-id="299e5-145">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="299e5-146">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="299e5-146">recordingInfo</span></span>        | [<span data-ttu-id="299e5-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="299e5-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="299e5-148">参加者が録画機能を持つかどうかについて説明します。</span><span class="sxs-lookup"><span data-stu-id="299e5-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="299e5-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="299e5-149">Relationships</span></span>
<span data-ttu-id="299e5-150">なし</span><span class="sxs-lookup"><span data-stu-id="299e5-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="299e5-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="299e5-151">JSON representation</span></span>

<span data-ttu-id="299e5-152">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="299e5-152">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "String (identifier)",
  "info": {"@odata.type": "#microsoft.graph.participantInfo"},
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ],
  "metadata": "String",
  "recordingInfo": { "@odata.type": "#microsoft.graph.recordingInfo" }
}
```

## <a name="example"></a><span data-ttu-id="299e5-153">例</span><span class="sxs-lookup"><span data-stu-id="299e5-153">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus"
  },
  "isInLobby": false,
  "isMuted": false,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "status": "recordingCapable"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/participant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
