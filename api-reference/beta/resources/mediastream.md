---
title: mediaStream リソースの種類
description: MediaStream 型です。
ms.openlocfilehash: 28eb98a3ab1be67c60c6ebd35deb7618f1618be3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074058"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="10e3a-103">mediaStream リソースの種類</span><span class="sxs-lookup"><span data-stu-id="10e3a-103">mediaStream resource type</span></span>

> <span data-ttu-id="10e3a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="10e3a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10e3a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10e3a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="10e3a-106">MediaStream 型です。</span><span class="sxs-lookup"><span data-stu-id="10e3a-106">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="10e3a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10e3a-107">Properties</span></span>

| <span data-ttu-id="10e3a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10e3a-108">Property</span></span>    | <span data-ttu-id="10e3a-109">型</span><span class="sxs-lookup"><span data-stu-id="10e3a-109">Type</span></span>    | <span data-ttu-id="10e3a-110">説明</span><span class="sxs-lookup"><span data-stu-id="10e3a-110">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="10e3a-111">方向</span><span class="sxs-lookup"><span data-stu-id="10e3a-111">direction</span></span>   | <span data-ttu-id="10e3a-112">String</span><span class="sxs-lookup"><span data-stu-id="10e3a-112">String</span></span>  | <span data-ttu-id="10e3a-113">方向です。</span><span class="sxs-lookup"><span data-stu-id="10e3a-113">The direction.</span></span> <span data-ttu-id="10e3a-114">使用可能な値は、 `inactive`、 `sendOnly`、 `receiveOnly`、 `sendReceive`。</span><span class="sxs-lookup"><span data-stu-id="10e3a-114">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="10e3a-115">label</span><span class="sxs-lookup"><span data-stu-id="10e3a-115">label</span></span>       | <span data-ttu-id="10e3a-116">String</span><span class="sxs-lookup"><span data-stu-id="10e3a-116">String</span></span>  | <span data-ttu-id="10e3a-117">メディア ストリームのラベルです。</span><span class="sxs-lookup"><span data-stu-id="10e3a-117">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="10e3a-118">メディアの種類</span><span class="sxs-lookup"><span data-stu-id="10e3a-118">mediaType</span></span>   | <span data-ttu-id="10e3a-119">String</span><span class="sxs-lookup"><span data-stu-id="10e3a-119">String</span></span>  | <span data-ttu-id="10e3a-120">メディアは次のとおり入力します。</span><span class="sxs-lookup"><span data-stu-id="10e3a-120">The media type.</span></span> <span data-ttu-id="10e3a-121">使用可能な値は、 `unknown`、 `audio`、 `video`、 `videoBasedScreenSharing`、 `data`。</span><span class="sxs-lookup"><span data-stu-id="10e3a-121">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="10e3a-122">serverMuted</span><span class="sxs-lookup"><span data-stu-id="10e3a-122">serverMuted</span></span> | <span data-ttu-id="10e3a-123">ブール値</span><span class="sxs-lookup"><span data-stu-id="10e3a-123">Boolean</span></span> | <span data-ttu-id="10e3a-124">サーバによってメディアがミュートされている場合。</span><span class="sxs-lookup"><span data-stu-id="10e3a-124">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="10e3a-125">sourceId</span><span class="sxs-lookup"><span data-stu-id="10e3a-125">sourceId</span></span>    | <span data-ttu-id="10e3a-126">String</span><span class="sxs-lookup"><span data-stu-id="10e3a-126">String</span></span>  | <span data-ttu-id="10e3a-127">ソースの id。</span><span class="sxs-lookup"><span data-stu-id="10e3a-127">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="10e3a-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="10e3a-128">JSON representation</span></span>

<span data-ttu-id="10e3a-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="10e3a-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="10e3a-130">使用例</span><span class="sxs-lookup"><span data-stu-id="10e3a-130">Example</span></span>

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
