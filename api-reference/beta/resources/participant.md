---
title: 参加者のリソースの種類
description: 参加者のタイプです。
author: VinodRavichandran
ms.openlocfilehash: 3fcc5fc5d95ded3b5424370cd180fde38c1a65be
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380395"
---
# <a name="participant-resource-type"></a><span data-ttu-id="4cb81-103">参加者のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="4cb81-103">participant resource type</span></span>

> <span data-ttu-id="4cb81-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4cb81-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4cb81-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4cb81-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4cb81-106">参加者のタイプです。</span><span class="sxs-lookup"><span data-stu-id="4cb81-106">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="4cb81-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4cb81-107">Methods</span></span>

| <span data-ttu-id="4cb81-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4cb81-108">Method</span></span>                                                          | <span data-ttu-id="4cb81-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4cb81-109">Return Type</span></span>                              | <span data-ttu-id="4cb81-110">説明</span><span class="sxs-lookup"><span data-stu-id="4cb81-110">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="4cb81-111">構成要素を取得します。</span><span class="sxs-lookup"><span data-stu-id="4cb81-111">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="4cb81-112">参加者</span><span class="sxs-lookup"><span data-stu-id="4cb81-112">participant</span></span>](participant.md)            | <span data-ttu-id="4cb81-113">**構成要素**オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="4cb81-113">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="4cb81-114">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="4cb81-114">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="4cb81-115">commsOperation</span><span class="sxs-lookup"><span data-stu-id="4cb81-115">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="4cb81-116">参加者のオーディオ ミキサーを構成します。</span><span class="sxs-lookup"><span data-stu-id="4cb81-116">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="4cb81-117">招待</span><span class="sxs-lookup"><span data-stu-id="4cb81-117">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="4cb81-118">commsOperation</span><span class="sxs-lookup"><span data-stu-id="4cb81-118">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="4cb81-119">通話に参加者を招待します。</span><span class="sxs-lookup"><span data-stu-id="4cb81-119">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="4cb81-120">参加者のミュート</span><span class="sxs-lookup"><span data-stu-id="4cb81-120">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="4cb81-121">commsOperation</span><span class="sxs-lookup"><span data-stu-id="4cb81-121">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="4cb81-122">呼び出し内の参加者をミュートします。</span><span class="sxs-lookup"><span data-stu-id="4cb81-122">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="4cb81-123">参加者全員をミュートします。</span><span class="sxs-lookup"><span data-stu-id="4cb81-123">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="4cb81-124">commsOperation</span><span class="sxs-lookup"><span data-stu-id="4cb81-124">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="4cb81-125">会議のすべての参加者をミュートします。</span><span class="sxs-lookup"><span data-stu-id="4cb81-125">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="4cb81-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4cb81-126">Properties</span></span>

| <span data-ttu-id="4cb81-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4cb81-127">Property</span></span>             | <span data-ttu-id="4cb81-128">型</span><span class="sxs-lookup"><span data-stu-id="4cb81-128">Type</span></span>                                     | <span data-ttu-id="4cb81-129">説明</span><span class="sxs-lookup"><span data-stu-id="4cb81-129">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="4cb81-130">id</span><span class="sxs-lookup"><span data-stu-id="4cb81-130">id</span></span>                   | <span data-ttu-id="4cb81-131">String</span><span class="sxs-lookup"><span data-stu-id="4cb81-131">String</span></span>                                   | <span data-ttu-id="4cb81-132">参加者の id です。</span><span class="sxs-lookup"><span data-stu-id="4cb81-132">The participant id.</span></span>                                          |
| <span data-ttu-id="4cb81-133">情報</span><span class="sxs-lookup"><span data-stu-id="4cb81-133">info</span></span>                 | [<span data-ttu-id="4cb81-134">participantInfo</span><span class="sxs-lookup"><span data-stu-id="4cb81-134">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="4cb81-135">参加者の参加者です。</span><span class="sxs-lookup"><span data-stu-id="4cb81-135">The participant of the participant.</span></span>                          |
| <span data-ttu-id="4cb81-136">isInLobby</span><span class="sxs-lookup"><span data-stu-id="4cb81-136">isInLobby</span></span>            | <span data-ttu-id="4cb81-137">ブール</span><span class="sxs-lookup"><span data-stu-id="4cb81-137">boolean</span></span>                                  | <span data-ttu-id="4cb81-138">参加者がロビーに入っている場合は true。</span><span class="sxs-lookup"><span data-stu-id="4cb81-138">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="4cb81-139">isMuted</span><span class="sxs-lookup"><span data-stu-id="4cb81-139">isMuted</span></span>              | <span data-ttu-id="4cb81-140">ブール</span><span class="sxs-lookup"><span data-stu-id="4cb81-140">boolean</span></span>                                  | <span data-ttu-id="4cb81-141">参加者がミュートされている場合は true (クライアントまたはサーバーがミュートになって)</span><span class="sxs-lookup"><span data-stu-id="4cb81-141">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="4cb81-142">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="4cb81-142">mediaStreams</span></span>         | <span data-ttu-id="4cb81-143">[mediaStream](mediastream.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4cb81-143">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="4cb81-144">メディア ストリームのリスト。</span><span class="sxs-lookup"><span data-stu-id="4cb81-144">The list of media streams.</span></span>                                   |
| <span data-ttu-id="4cb81-145">metadata</span><span class="sxs-lookup"><span data-stu-id="4cb81-145">metadata</span></span>             | <span data-ttu-id="4cb81-146">String</span><span class="sxs-lookup"><span data-stu-id="4cb81-146">String</span></span>                                   | <span data-ttu-id="4cb81-147">名簿にある参加者が提供するデータの blob</span><span class="sxs-lookup"><span data-stu-id="4cb81-147">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="4cb81-148">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="4cb81-148">recordingInfo</span></span>        | [<span data-ttu-id="4cb81-149">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="4cb81-149">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="4cb81-150">参加者が録画機能を持つかどうかについて説明します。</span><span class="sxs-lookup"><span data-stu-id="4cb81-150">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4cb81-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4cb81-151">Relationships</span></span>
<span data-ttu-id="4cb81-152">なし</span><span class="sxs-lookup"><span data-stu-id="4cb81-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cb81-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4cb81-153">JSON representation</span></span>

<span data-ttu-id="4cb81-154">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4cb81-154">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="4cb81-155">例</span><span class="sxs-lookup"><span data-stu-id="4cb81-155">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->