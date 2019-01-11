---
title: timeZoneBase リソースの種類
description: タイム ゾーンの基本的な表現です。
localization_priority: Normal
ms.openlocfilehash: 4c112a3118bf3f4d00be790d7923bc0fe82dc72f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860635"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="b3fe9-103">timeZoneBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3fe9-103">timeZoneBase resource type</span></span>

<span data-ttu-id="b3fe9-104">タイム ゾーンの基本的な表現です。</span><span class="sxs-lookup"><span data-stu-id="b3fe9-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="b3fe9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3fe9-105">Properties</span></span>
| <span data-ttu-id="b3fe9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3fe9-106">Property</span></span>     | <span data-ttu-id="b3fe9-107">種類</span><span class="sxs-lookup"><span data-stu-id="b3fe9-107">Type</span></span>   |<span data-ttu-id="b3fe9-108">説明</span><span class="sxs-lookup"><span data-stu-id="b3fe9-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b3fe9-109">name</span><span class="sxs-lookup"><span data-stu-id="b3fe9-109">name</span></span> | <span data-ttu-id="b3fe9-110">文字列</span><span class="sxs-lookup"><span data-stu-id="b3fe9-110">string</span></span> | <span data-ttu-id="b3fe9-111">タイム ゾーンの名前。</span><span class="sxs-lookup"><span data-stu-id="b3fe9-111">The name of a time zone.</span></span> <span data-ttu-id="b3fe9-112">標準的なタイム ゾーンの名前 ("ハワイ アリューシャン標準時" など) を使用することも、カスタム タイム ゾーンとして "カスタム タイム ゾーン" という名前を指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="b3fe9-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b3fe9-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3fe9-113">JSON representation</span></span>

<span data-ttu-id="b3fe9-114">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3fe9-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
