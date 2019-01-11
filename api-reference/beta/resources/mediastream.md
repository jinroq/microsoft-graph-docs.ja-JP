---
title: mediaStream リソースの種類
description: MediaStream 型です。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 7e56448c2c6d284e7a5904f1b0af414166782907
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889615"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="274db-103">mediaStream リソースの種類</span><span class="sxs-lookup"><span data-stu-id="274db-103">mediaStream resource type</span></span>

> <span data-ttu-id="274db-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="274db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="274db-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="274db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="274db-106">MediaStream 型です。</span><span class="sxs-lookup"><span data-stu-id="274db-106">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="274db-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="274db-107">Properties</span></span>

| <span data-ttu-id="274db-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="274db-108">Property</span></span>    | <span data-ttu-id="274db-109">種類</span><span class="sxs-lookup"><span data-stu-id="274db-109">Type</span></span>    | <span data-ttu-id="274db-110">説明</span><span class="sxs-lookup"><span data-stu-id="274db-110">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="274db-111">方向</span><span class="sxs-lookup"><span data-stu-id="274db-111">direction</span></span>   | <span data-ttu-id="274db-112">String</span><span class="sxs-lookup"><span data-stu-id="274db-112">String</span></span>  | <span data-ttu-id="274db-113">方向です。</span><span class="sxs-lookup"><span data-stu-id="274db-113">The direction.</span></span> <span data-ttu-id="274db-114">使用可能な値は、 `inactive`、 `sendOnly`、 `receiveOnly`、 `sendReceive`。</span><span class="sxs-lookup"><span data-stu-id="274db-114">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="274db-115">label</span><span class="sxs-lookup"><span data-stu-id="274db-115">label</span></span>       | <span data-ttu-id="274db-116">String</span><span class="sxs-lookup"><span data-stu-id="274db-116">String</span></span>  | <span data-ttu-id="274db-117">メディア ストリームのラベルです。</span><span class="sxs-lookup"><span data-stu-id="274db-117">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="274db-118">メディアの種類</span><span class="sxs-lookup"><span data-stu-id="274db-118">mediaType</span></span>   | <span data-ttu-id="274db-119">String</span><span class="sxs-lookup"><span data-stu-id="274db-119">String</span></span>  | <span data-ttu-id="274db-120">メディアは次のとおり入力します。</span><span class="sxs-lookup"><span data-stu-id="274db-120">The media type.</span></span> <span data-ttu-id="274db-121">使用可能な値は、 `unknown`、 `audio`、 `video`、 `videoBasedScreenSharing`、 `data`。</span><span class="sxs-lookup"><span data-stu-id="274db-121">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="274db-122">serverMuted</span><span class="sxs-lookup"><span data-stu-id="274db-122">serverMuted</span></span> | <span data-ttu-id="274db-123">ブール型</span><span class="sxs-lookup"><span data-stu-id="274db-123">Boolean</span></span> | <span data-ttu-id="274db-124">サーバによってメディアがミュートされている場合。</span><span class="sxs-lookup"><span data-stu-id="274db-124">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="274db-125">sourceId</span><span class="sxs-lookup"><span data-stu-id="274db-125">sourceId</span></span>    | <span data-ttu-id="274db-126">String</span><span class="sxs-lookup"><span data-stu-id="274db-126">String</span></span>  | <span data-ttu-id="274db-127">ソースの id。</span><span class="sxs-lookup"><span data-stu-id="274db-127">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="274db-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="274db-128">JSON representation</span></span>

<span data-ttu-id="274db-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="274db-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted"
  ],
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "inactive | sendOnly | receiveOnly | sendReceive",
  "label": "String",
  "mediaType": "unknown | audio | video | videoBasedScreenSharing | data",
  "serverMuted": true,
  "sourceId": "String"
}
```

## <a name="example"></a><span data-ttu-id="274db-130">例</span><span class="sxs-lookup"><span data-stu-id="274db-130">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "sendReceive",
  "label": "main-audio",
  "mediaType": "audio",
  "serverMuted": false,
  "sourceId": "1024"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
