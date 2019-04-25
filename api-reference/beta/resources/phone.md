---
title: phone リソースの種類
description: 電話番号を表します。
localization_priority: Normal
ms.openlocfilehash: a343d4e1d65126048a27ad723c86ae49eb2ed752
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573768"
---
# <a name="phone-resource-type"></a><span data-ttu-id="5a8c9-103">phone リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a8c9-103">phone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a8c9-104">電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="5a8c9-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="5a8c9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a8c9-105">Properties</span></span>
| <span data-ttu-id="5a8c9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a8c9-106">Property</span></span>     | <span data-ttu-id="5a8c9-107">型</span><span class="sxs-lookup"><span data-stu-id="5a8c9-107">Type</span></span>   |<span data-ttu-id="5a8c9-108">説明</span><span class="sxs-lookup"><span data-stu-id="5a8c9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a8c9-109">番号</span><span class="sxs-lookup"><span data-stu-id="5a8c9-109">number</span></span>|<span data-ttu-id="5a8c9-110">string</span><span class="sxs-lookup"><span data-stu-id="5a8c9-110">string</span></span>|<span data-ttu-id="5a8c9-111">電話番号。</span><span class="sxs-lookup"><span data-stu-id="5a8c9-111">The phone number.</span></span>|
|<span data-ttu-id="5a8c9-112">type</span><span class="sxs-lookup"><span data-stu-id="5a8c9-112">type</span></span>|<span data-ttu-id="5a8c9-113">String</span><span class="sxs-lookup"><span data-stu-id="5a8c9-113">String</span></span>|<span data-ttu-id="5a8c9-p101">電話番号の種類。 可能な値は、`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio` です。</span><span class="sxs-lookup"><span data-stu-id="5a8c9-p101">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a8c9-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a8c9-116">JSON representation</span></span>

<span data-ttu-id="5a8c9-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a8c9-117">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/phone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
