---
title: mediaStream リソースの種類
description: MediaStream の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c39c4eb0754f327361fec04852293ef084b0c412
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966827"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="b4539-103">mediaStream リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b4539-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4539-104">MediaStream の種類。</span><span class="sxs-lookup"><span data-stu-id="b4539-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="b4539-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4539-105">Properties</span></span>

| <span data-ttu-id="b4539-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4539-106">Property</span></span>    | <span data-ttu-id="b4539-107">型</span><span class="sxs-lookup"><span data-stu-id="b4539-107">Type</span></span>    | <span data-ttu-id="b4539-108">説明</span><span class="sxs-lookup"><span data-stu-id="b4539-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="b4539-109">direction</span><span class="sxs-lookup"><span data-stu-id="b4539-109">direction</span></span>   | <span data-ttu-id="b4539-110">String</span><span class="sxs-lookup"><span data-stu-id="b4539-110">String</span></span>  | <span data-ttu-id="b4539-111">方向を示します。</span><span class="sxs-lookup"><span data-stu-id="b4539-111">The direction.</span></span> <span data-ttu-id="b4539-112">使用可能な値`inactive`は`sendOnly` `receiveOnly`、、 `sendReceive`、です。</span><span class="sxs-lookup"><span data-stu-id="b4539-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="b4539-113">label</span><span class="sxs-lookup"><span data-stu-id="b4539-113">label</span></span>       | <span data-ttu-id="b4539-114">String</span><span class="sxs-lookup"><span data-stu-id="b4539-114">String</span></span>  | <span data-ttu-id="b4539-115">メディアストリームのラベル。</span><span class="sxs-lookup"><span data-stu-id="b4539-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="b4539-116">mediaType</span><span class="sxs-lookup"><span data-stu-id="b4539-116">mediaType</span></span>   | <span data-ttu-id="b4539-117">String</span><span class="sxs-lookup"><span data-stu-id="b4539-117">String</span></span>  | <span data-ttu-id="b4539-118">メディアの種類。</span><span class="sxs-lookup"><span data-stu-id="b4539-118">The media type.</span></span> <span data-ttu-id="b4539-119">使用可能な値`unknown`は`audio` `video` `videoBasedScreenSharing`、、、 `data`、です。</span><span class="sxs-lookup"><span data-stu-id="b4539-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="b4539-120">serverMuted</span><span class="sxs-lookup"><span data-stu-id="b4539-120">serverMuted</span></span> | <span data-ttu-id="b4539-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4539-121">Boolean</span></span> | <span data-ttu-id="b4539-122">メディアがサーバーによってミュートされている場合。</span><span class="sxs-lookup"><span data-stu-id="b4539-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="b4539-123">sourceId</span><span class="sxs-lookup"><span data-stu-id="b4539-123">sourceId</span></span>    | <span data-ttu-id="b4539-124">String</span><span class="sxs-lookup"><span data-stu-id="b4539-124">String</span></span>  | <span data-ttu-id="b4539-125">ソース ID。</span><span class="sxs-lookup"><span data-stu-id="b4539-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="b4539-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b4539-126">JSON representation</span></span>

<span data-ttu-id="b4539-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b4539-127">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b4539-128">例</span><span class="sxs-lookup"><span data-stu-id="b4539-128">Example</span></span>

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
  "suppressions": []
}
-->
