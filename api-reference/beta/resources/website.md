---
title: Web サイトのリソースの種類
description: Web サイトを表します。
localization_priority: Normal
ms.openlocfilehash: 3f8aadaf0a6b6beb2394664f04195267062dc9ae
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511227"
---
# <a name="website-resource-type"></a><span data-ttu-id="43d32-103">Web サイトのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="43d32-103">website resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43d32-104">Web サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="43d32-104">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="43d32-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43d32-105">Properties</span></span>
| <span data-ttu-id="43d32-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43d32-106">Property</span></span>     | <span data-ttu-id="43d32-107">型</span><span class="sxs-lookup"><span data-stu-id="43d32-107">Type</span></span>   |<span data-ttu-id="43d32-108">説明</span><span class="sxs-lookup"><span data-stu-id="43d32-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43d32-109">type</span><span class="sxs-lookup"><span data-stu-id="43d32-109">type</span></span>|<span data-ttu-id="43d32-110">String</span><span class="sxs-lookup"><span data-stu-id="43d32-110">String</span></span>| <span data-ttu-id="43d32-111">可能な値は、`other`、`home`、`work`、`blog`、`profile` です。</span><span class="sxs-lookup"><span data-stu-id="43d32-111">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="43d32-112">アドレス</span><span class="sxs-lookup"><span data-stu-id="43d32-112">address</span></span>|<span data-ttu-id="43d32-113">string</span><span class="sxs-lookup"><span data-stu-id="43d32-113">string</span></span>|<span data-ttu-id="43d32-114">Web サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="43d32-114">The URL of the website.</span></span>|
|<span data-ttu-id="43d32-115">displayName</span><span class="sxs-lookup"><span data-stu-id="43d32-115">displayName</span></span>|<span data-ttu-id="43d32-116">string</span><span class="sxs-lookup"><span data-stu-id="43d32-116">string</span></span>|<span data-ttu-id="43d32-117">Web サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="43d32-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43d32-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43d32-118">JSON representation</span></span>

<span data-ttu-id="43d32-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="43d32-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/website.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
