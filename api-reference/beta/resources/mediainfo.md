---
title: mediaInfo リソースの種類
description: アクションで使用されるメディアの情報には次のメッセージが表示されます。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 217b9a5aaa88a1bbf343447fad344b322cfeb611
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924532"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="5c9c3-103">mediaInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5c9c3-103">mediaInfo resource type</span></span>

> <span data-ttu-id="5c9c3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5c9c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c9c3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c9c3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c9c3-106">アクションで使用されるメディアの情報には次のメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="5c9c3-106">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="5c9c3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c9c3-107">Properties</span></span>
| <span data-ttu-id="5c9c3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c9c3-108">Property</span></span>       | <span data-ttu-id="5c9c3-109">種類</span><span class="sxs-lookup"><span data-stu-id="5c9c3-109">Type</span></span>    | <span data-ttu-id="5c9c3-110">説明</span><span class="sxs-lookup"><span data-stu-id="5c9c3-110">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="5c9c3-111">resourceId</span><span class="sxs-lookup"><span data-stu-id="5c9c3-111">resourceId</span></span>     | <span data-ttu-id="5c9c3-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5c9c3-112">String</span></span>  | <span data-ttu-id="5c9c3-113">リソースの一意の id。</span><span class="sxs-lookup"><span data-stu-id="5c9c3-113">Unique identity of the resource.</span></span> |
| <span data-ttu-id="5c9c3-114">uri</span><span class="sxs-lookup"><span data-stu-id="5c9c3-114">uri</span></span>            | <span data-ttu-id="5c9c3-115">String</span><span class="sxs-lookup"><span data-stu-id="5c9c3-115">String</span></span>  | <span data-ttu-id="5c9c3-116">リソースへのパス。</span><span class="sxs-lookup"><span data-stu-id="5c9c3-116">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="5c9c3-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c9c3-117">JSON representation</span></span>

<span data-ttu-id="5c9c3-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5c9c3-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
