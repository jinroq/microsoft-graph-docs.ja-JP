---
title: 電話リソースの種類
description: 電話番号を表します。
localization_priority: Normal
ms.openlocfilehash: 6c34033b0895f81619589e7500441fc655842995
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805062"
---
# <a name="phone-resource-type"></a><span data-ttu-id="b2e9f-103">電話リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2e9f-103">phone resource type</span></span>

<span data-ttu-id="b2e9f-104">電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="b2e9f-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="b2e9f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2e9f-105">Properties</span></span>
| <span data-ttu-id="b2e9f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2e9f-106">Property</span></span>     | <span data-ttu-id="b2e9f-107">種類</span><span class="sxs-lookup"><span data-stu-id="b2e9f-107">Type</span></span>   |<span data-ttu-id="b2e9f-108">説明</span><span class="sxs-lookup"><span data-stu-id="b2e9f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2e9f-109">number</span><span class="sxs-lookup"><span data-stu-id="b2e9f-109">number</span></span>|<span data-ttu-id="b2e9f-110">文字列</span><span class="sxs-lookup"><span data-stu-id="b2e9f-110">string</span></span>|<span data-ttu-id="b2e9f-111">電話番号。</span><span class="sxs-lookup"><span data-stu-id="b2e9f-111">The phone number.</span></span>|
|<span data-ttu-id="b2e9f-112">種類</span><span class="sxs-lookup"><span data-stu-id="b2e9f-112">type</span></span>|<span data-ttu-id="b2e9f-113">phoneType</span><span class="sxs-lookup"><span data-stu-id="b2e9f-113">phoneType</span></span>|<span data-ttu-id="b2e9f-114">電話番号の種類。</span><span class="sxs-lookup"><span data-stu-id="b2e9f-114">The type of phone number.</span></span> <span data-ttu-id="b2e9f-115">可能な値: `home`、 `business`、 `mobile`、 `other`、 `assistant`、 `homeFax`、 `businessFax`、 `otherFax`、 `pager`、 `radio`。</span><span class="sxs-lookup"><span data-stu-id="b2e9f-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2e9f-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2e9f-116">JSON representation</span></span>

<span data-ttu-id="b2e9f-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b2e9f-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
