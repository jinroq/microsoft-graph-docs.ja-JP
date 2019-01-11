---
title: mediaInfo リソースの種類
description: アクションで使用されるメディアの情報には次のメッセージが表示されます。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 6fe2c49e86bac9d5961310694b21e9439a4896ab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885604"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="2c250-103">mediaInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c250-103">mediaInfo resource type</span></span>

> <span data-ttu-id="2c250-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2c250-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c250-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c250-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2c250-106">アクションで使用されるメディアの情報には次のメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="2c250-106">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="2c250-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c250-107">Properties</span></span>
| <span data-ttu-id="2c250-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c250-108">Property</span></span>       | <span data-ttu-id="2c250-109">種類</span><span class="sxs-lookup"><span data-stu-id="2c250-109">Type</span></span>    | <span data-ttu-id="2c250-110">説明</span><span class="sxs-lookup"><span data-stu-id="2c250-110">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="2c250-111">resourceId</span><span class="sxs-lookup"><span data-stu-id="2c250-111">resourceId</span></span>     | <span data-ttu-id="2c250-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2c250-112">String</span></span>  | <span data-ttu-id="2c250-113">リソースの一意の id。</span><span class="sxs-lookup"><span data-stu-id="2c250-113">Unique identity of the resource.</span></span> |
| <span data-ttu-id="2c250-114">uri</span><span class="sxs-lookup"><span data-stu-id="2c250-114">uri</span></span>            | <span data-ttu-id="2c250-115">String</span><span class="sxs-lookup"><span data-stu-id="2c250-115">String</span></span>  | <span data-ttu-id="2c250-116">リソースへのパス。</span><span class="sxs-lookup"><span data-stu-id="2c250-116">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="2c250-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c250-117">JSON representation</span></span>

<span data-ttu-id="2c250-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2c250-118">The following is a JSON representation of the resource.</span></span>

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
