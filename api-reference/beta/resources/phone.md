---
title: phone リソースの種類
description: 電話番号を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ad7438e532420d15f14096a0843b42456a4b1fbc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966121"
---
# <a name="phone-resource-type"></a><span data-ttu-id="6fa27-103">phone リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6fa27-103">phone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fa27-104">電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="6fa27-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="6fa27-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fa27-105">Properties</span></span>
| <span data-ttu-id="6fa27-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fa27-106">Property</span></span>     | <span data-ttu-id="6fa27-107">型</span><span class="sxs-lookup"><span data-stu-id="6fa27-107">Type</span></span>   |<span data-ttu-id="6fa27-108">説明</span><span class="sxs-lookup"><span data-stu-id="6fa27-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fa27-109">番号</span><span class="sxs-lookup"><span data-stu-id="6fa27-109">number</span></span>|<span data-ttu-id="6fa27-110">string</span><span class="sxs-lookup"><span data-stu-id="6fa27-110">string</span></span>|<span data-ttu-id="6fa27-111">電話番号。</span><span class="sxs-lookup"><span data-stu-id="6fa27-111">The phone number.</span></span>|
|<span data-ttu-id="6fa27-112">type</span><span class="sxs-lookup"><span data-stu-id="6fa27-112">type</span></span>|<span data-ttu-id="6fa27-113">String</span><span class="sxs-lookup"><span data-stu-id="6fa27-113">String</span></span>|<span data-ttu-id="6fa27-p101">電話番号の種類。 可能な値は、`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio` です。</span><span class="sxs-lookup"><span data-stu-id="6fa27-p101">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fa27-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6fa27-116">JSON representation</span></span>

<span data-ttu-id="6fa27-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6fa27-117">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
