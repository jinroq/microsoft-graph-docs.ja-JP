---
title: 電話リソースの種類
description: 電話番号を表します。
ms.openlocfilehash: 1293b1f84d9e73f5d92c9b6f6b078b5f39126e33
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023191"
---
# <a name="phone-resource-type"></a><span data-ttu-id="7cd85-103">電話リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7cd85-103">phone resource type</span></span>

<span data-ttu-id="7cd85-104">電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="7cd85-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="7cd85-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cd85-105">Properties</span></span>
| <span data-ttu-id="7cd85-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cd85-106">Property</span></span>     | <span data-ttu-id="7cd85-107">型</span><span class="sxs-lookup"><span data-stu-id="7cd85-107">Type</span></span>   |<span data-ttu-id="7cd85-108">説明</span><span class="sxs-lookup"><span data-stu-id="7cd85-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cd85-109">数値</span><span class="sxs-lookup"><span data-stu-id="7cd85-109">number</span></span>|<span data-ttu-id="7cd85-110">文字列</span><span class="sxs-lookup"><span data-stu-id="7cd85-110">string</span></span>|<span data-ttu-id="7cd85-111">電話番号。</span><span class="sxs-lookup"><span data-stu-id="7cd85-111">The phone number.</span></span>|
|<span data-ttu-id="7cd85-112">種類</span><span class="sxs-lookup"><span data-stu-id="7cd85-112">type</span></span>|<span data-ttu-id="7cd85-113">phoneType</span><span class="sxs-lookup"><span data-stu-id="7cd85-113">phoneType</span></span>|<span data-ttu-id="7cd85-114">電話番号の種類。</span><span class="sxs-lookup"><span data-stu-id="7cd85-114">The type of phone number.</span></span> <span data-ttu-id="7cd85-115">可能な値: `home`、 `business`、 `mobile`、 `other`、 `assistant`、 `homeFax`、 `businessFax`、 `otherFax`、 `pager`、 `radio`。</span><span class="sxs-lookup"><span data-stu-id="7cd85-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7cd85-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7cd85-116">JSON representation</span></span>

<span data-ttu-id="7cd85-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7cd85-117">Here is a JSON representation of the resource.</span></span>

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
