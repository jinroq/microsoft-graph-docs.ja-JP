---
title: mediaInfo リソースの種類
description: アクションで使用されるメディアの情報には次のメッセージが表示されます。
author: VinodRavichandran
ms.openlocfilehash: ea2eaa9e8e85da737df4c0c0170457fb3350820b
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380276"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="45f7c-103">mediaInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="45f7c-103">mediaInfo resource type</span></span>

> <span data-ttu-id="45f7c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="45f7c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45f7c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45f7c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="45f7c-106">アクションで使用されるメディアの情報には次のメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="45f7c-106">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="45f7c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45f7c-107">Properties</span></span>
| <span data-ttu-id="45f7c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45f7c-108">Property</span></span>       | <span data-ttu-id="45f7c-109">型</span><span class="sxs-lookup"><span data-stu-id="45f7c-109">Type</span></span>    | <span data-ttu-id="45f7c-110">説明</span><span class="sxs-lookup"><span data-stu-id="45f7c-110">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="45f7c-111">resourceId</span><span class="sxs-lookup"><span data-stu-id="45f7c-111">resourceId</span></span>     | <span data-ttu-id="45f7c-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="45f7c-112">String</span></span>  | <span data-ttu-id="45f7c-113">リソースの一意の id。</span><span class="sxs-lookup"><span data-stu-id="45f7c-113">Unique identity of the resource.</span></span> |
| <span data-ttu-id="45f7c-114">uri</span><span class="sxs-lookup"><span data-stu-id="45f7c-114">uri</span></span>            | <span data-ttu-id="45f7c-115">String</span><span class="sxs-lookup"><span data-stu-id="45f7c-115">String</span></span>  | <span data-ttu-id="45f7c-116">リソースへのパス。</span><span class="sxs-lookup"><span data-stu-id="45f7c-116">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="45f7c-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="45f7c-117">JSON representation</span></span>

<span data-ttu-id="45f7c-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="45f7c-118">The following is a JSON representation of the resource.</span></span>

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