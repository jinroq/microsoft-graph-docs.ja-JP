---
title: mediastream リソースの種類
description: mediastream の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4867675da3427beb790beb240cd7bc0b86f04317
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581580"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="48e6e-103">mediastream リソースの種類</span><span class="sxs-lookup"><span data-stu-id="48e6e-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48e6e-104">mediastream の種類。</span><span class="sxs-lookup"><span data-stu-id="48e6e-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="48e6e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48e6e-105">Properties</span></span>

| <span data-ttu-id="48e6e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48e6e-106">Property</span></span>    | <span data-ttu-id="48e6e-107">型</span><span class="sxs-lookup"><span data-stu-id="48e6e-107">Type</span></span>    | <span data-ttu-id="48e6e-108">説明</span><span class="sxs-lookup"><span data-stu-id="48e6e-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="48e6e-109">direction</span><span class="sxs-lookup"><span data-stu-id="48e6e-109">direction</span></span>   | <span data-ttu-id="48e6e-110">String</span><span class="sxs-lookup"><span data-stu-id="48e6e-110">String</span></span>  | <span data-ttu-id="48e6e-111">方向を示します。</span><span class="sxs-lookup"><span data-stu-id="48e6e-111">The direction.</span></span> <span data-ttu-id="48e6e-112">使用可能な値`inactive`は`sendOnly` `receiveOnly`、、 `sendReceive`、です。</span><span class="sxs-lookup"><span data-stu-id="48e6e-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="48e6e-113">label</span><span class="sxs-lookup"><span data-stu-id="48e6e-113">label</span></span>       | <span data-ttu-id="48e6e-114">String</span><span class="sxs-lookup"><span data-stu-id="48e6e-114">String</span></span>  | <span data-ttu-id="48e6e-115">メディアストリームのラベル。</span><span class="sxs-lookup"><span data-stu-id="48e6e-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="48e6e-116">mediaType</span><span class="sxs-lookup"><span data-stu-id="48e6e-116">mediaType</span></span>   | <span data-ttu-id="48e6e-117">String</span><span class="sxs-lookup"><span data-stu-id="48e6e-117">String</span></span>  | <span data-ttu-id="48e6e-118">メディアの種類。</span><span class="sxs-lookup"><span data-stu-id="48e6e-118">The media type.</span></span> <span data-ttu-id="48e6e-119">使用可能な値`unknown`は`audio` `video` `videoBasedScreenSharing`、、、 `data`、です。</span><span class="sxs-lookup"><span data-stu-id="48e6e-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="48e6e-120">servermuted</span><span class="sxs-lookup"><span data-stu-id="48e6e-120">serverMuted</span></span> | <span data-ttu-id="48e6e-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="48e6e-121">Boolean</span></span> | <span data-ttu-id="48e6e-122">メディアがサーバーによってミュートされている場合。</span><span class="sxs-lookup"><span data-stu-id="48e6e-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="48e6e-123">sourceId</span><span class="sxs-lookup"><span data-stu-id="48e6e-123">sourceId</span></span>    | <span data-ttu-id="48e6e-124">String</span><span class="sxs-lookup"><span data-stu-id="48e6e-124">String</span></span>  | <span data-ttu-id="48e6e-125">ソース ID。</span><span class="sxs-lookup"><span data-stu-id="48e6e-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="48e6e-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48e6e-126">JSON representation</span></span>

<span data-ttu-id="48e6e-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="48e6e-127">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="48e6e-128">例</span><span class="sxs-lookup"><span data-stu-id="48e6e-128">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mediastream.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
