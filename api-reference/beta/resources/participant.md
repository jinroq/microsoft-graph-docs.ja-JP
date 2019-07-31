---
title: 参加者リソースの種類
description: 参加者の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a903eb34191401100d9b19aa17eba6fb9f5c6617
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009217"
---
# <a name="participant-resource-type"></a><span data-ttu-id="8ad42-103">参加者リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ad42-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ad42-104">参加者の種類。</span><span class="sxs-lookup"><span data-stu-id="8ad42-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="8ad42-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="8ad42-105">Methods</span></span>

| <span data-ttu-id="8ad42-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8ad42-106">Method</span></span>                                                          | <span data-ttu-id="8ad42-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8ad42-107">Return Type</span></span>                              | <span data-ttu-id="8ad42-108">説明</span><span class="sxs-lookup"><span data-stu-id="8ad42-108">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="8ad42-109">参加者を取得する</span><span class="sxs-lookup"><span data-stu-id="8ad42-109">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="8ad42-110">積極的</span><span class="sxs-lookup"><span data-stu-id="8ad42-110">participant</span></span>](participant.md)            | <span data-ttu-id="8ad42-111">**参加者**オブジェクトのプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8ad42-111">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="8ad42-112">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="8ad42-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="8ad42-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8ad42-113">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8ad42-114">参加者のオーディオミキサーを構成します。</span><span class="sxs-lookup"><span data-stu-id="8ad42-114">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="8ad42-115">招待</span><span class="sxs-lookup"><span data-stu-id="8ad42-115">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="8ad42-116">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8ad42-116">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8ad42-117">参加者を呼び出しに招待します。</span><span class="sxs-lookup"><span data-stu-id="8ad42-117">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="8ad42-118">参加者をミュートする</span><span class="sxs-lookup"><span data-stu-id="8ad42-118">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="8ad42-119">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8ad42-119">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8ad42-120">通話の参加者をミュートにします。</span><span class="sxs-lookup"><span data-stu-id="8ad42-120">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="8ad42-121">すべての参加者をミュートする</span><span class="sxs-lookup"><span data-stu-id="8ad42-121">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="8ad42-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8ad42-122">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8ad42-123">会議のすべての参加者をミュートにします。</span><span class="sxs-lookup"><span data-stu-id="8ad42-123">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="8ad42-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ad42-124">Properties</span></span>

| <span data-ttu-id="8ad42-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ad42-125">Property</span></span>             | <span data-ttu-id="8ad42-126">型</span><span class="sxs-lookup"><span data-stu-id="8ad42-126">Type</span></span>                                     | <span data-ttu-id="8ad42-127">説明</span><span class="sxs-lookup"><span data-stu-id="8ad42-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="8ad42-128">id</span><span class="sxs-lookup"><span data-stu-id="8ad42-128">id</span></span>                   | <span data-ttu-id="8ad42-129">String</span><span class="sxs-lookup"><span data-stu-id="8ad42-129">String</span></span>                                   | <span data-ttu-id="8ad42-130">参加者 id。</span><span class="sxs-lookup"><span data-stu-id="8ad42-130">The participant id.</span></span>                                          |
| <span data-ttu-id="8ad42-131">info</span><span class="sxs-lookup"><span data-stu-id="8ad42-131">info</span></span>                 | [<span data-ttu-id="8ad42-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="8ad42-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="8ad42-133">参加者の参加者。</span><span class="sxs-lookup"><span data-stu-id="8ad42-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="8ad42-134">isInLobby</span><span class="sxs-lookup"><span data-stu-id="8ad42-134">isInLobby</span></span>            | <span data-ttu-id="8ad42-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ad42-135">boolean</span></span>                                  | <span data-ttu-id="8ad42-136">参加者がロビーにある場合は true</span><span class="sxs-lookup"><span data-stu-id="8ad42-136">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="8ad42-137">isMuted</span><span class="sxs-lookup"><span data-stu-id="8ad42-137">isMuted</span></span>              | <span data-ttu-id="8ad42-138">ブール値</span><span class="sxs-lookup"><span data-stu-id="8ad42-138">boolean</span></span>                                  | <span data-ttu-id="8ad42-139">参加者がミュートされている場合は true (クライアントまたはサーバーがミュート状態)</span><span class="sxs-lookup"><span data-stu-id="8ad42-139">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="8ad42-140">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="8ad42-140">mediaStreams</span></span>         | <span data-ttu-id="8ad42-141">[Mediastream](mediastream.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8ad42-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="8ad42-142">メディアストリームのリスト。</span><span class="sxs-lookup"><span data-stu-id="8ad42-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="8ad42-143">metadata</span><span class="sxs-lookup"><span data-stu-id="8ad42-143">metadata</span></span>             | <span data-ttu-id="8ad42-144">String</span><span class="sxs-lookup"><span data-stu-id="8ad42-144">String</span></span>                                   | <span data-ttu-id="8ad42-145">参加者が名簿に提供するデータの blob</span><span class="sxs-lookup"><span data-stu-id="8ad42-145">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="8ad42-146">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="8ad42-146">recordingInfo</span></span>        | [<span data-ttu-id="8ad42-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="8ad42-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="8ad42-148">参加者にレコーディング機能があるかどうかに関する情報。</span><span class="sxs-lookup"><span data-stu-id="8ad42-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8ad42-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8ad42-149">Relationships</span></span>
<span data-ttu-id="8ad42-150">なし</span><span class="sxs-lookup"><span data-stu-id="8ad42-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ad42-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ad42-151">JSON representation</span></span>

<span data-ttu-id="8ad42-152">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ad42-152">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="8ad42-153">例</span><span class="sxs-lookup"><span data-stu-id="8ad42-153">Example</span></span>

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
  "suppressions": []
}
-->
