---
title: mediaInfo リソースの種類
description: プロンプトのアクションで使用されるメディア情報。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 65cf71f5c116fe213d0e32d560ec24704bff1172
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562618"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="f59f7-103">mediaInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f59f7-103">mediaInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f59f7-104">プロンプトのアクションで使用されるメディア情報。</span><span class="sxs-lookup"><span data-stu-id="f59f7-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="f59f7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f59f7-105">Properties</span></span>
| <span data-ttu-id="f59f7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f59f7-106">Property</span></span>       | <span data-ttu-id="f59f7-107">型</span><span class="sxs-lookup"><span data-stu-id="f59f7-107">Type</span></span>    | <span data-ttu-id="f59f7-108">説明</span><span class="sxs-lookup"><span data-stu-id="f59f7-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="f59f7-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="f59f7-109">resourceId</span></span>     | <span data-ttu-id="f59f7-110">String</span><span class="sxs-lookup"><span data-stu-id="f59f7-110">String</span></span>  | <span data-ttu-id="f59f7-111">リソースの一意の id です。</span><span class="sxs-lookup"><span data-stu-id="f59f7-111">Unique identity of the resource.</span></span> |
| <span data-ttu-id="f59f7-112">uri</span><span class="sxs-lookup"><span data-stu-id="f59f7-112">uri</span></span>            | <span data-ttu-id="f59f7-113">String</span><span class="sxs-lookup"><span data-stu-id="f59f7-113">String</span></span>  | <span data-ttu-id="f59f7-114">リソースへのパス。</span><span class="sxs-lookup"><span data-stu-id="f59f7-114">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="f59f7-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f59f7-115">JSON representation</span></span>

<span data-ttu-id="f59f7-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f59f7-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
