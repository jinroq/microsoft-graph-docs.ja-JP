---
title: web サイトリソースの種類
description: Web サイトを表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0f822c38c57d5e47d39a40b3285773e0e36fd2ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964143"
---
# <a name="website-resource-type"></a><span data-ttu-id="ccbf7-103">web サイトリソースの種類</span><span class="sxs-lookup"><span data-stu-id="ccbf7-103">website resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccbf7-104">Web サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="ccbf7-104">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="ccbf7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccbf7-105">Properties</span></span>
| <span data-ttu-id="ccbf7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccbf7-106">Property</span></span>     | <span data-ttu-id="ccbf7-107">型</span><span class="sxs-lookup"><span data-stu-id="ccbf7-107">Type</span></span>   |<span data-ttu-id="ccbf7-108">説明</span><span class="sxs-lookup"><span data-stu-id="ccbf7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccbf7-109">type</span><span class="sxs-lookup"><span data-stu-id="ccbf7-109">type</span></span>|<span data-ttu-id="ccbf7-110">String</span><span class="sxs-lookup"><span data-stu-id="ccbf7-110">String</span></span>| <span data-ttu-id="ccbf7-111">可能な値は、`other`、`home`、`work`、`blog`、`profile` です。</span><span class="sxs-lookup"><span data-stu-id="ccbf7-111">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="ccbf7-112">address</span><span class="sxs-lookup"><span data-stu-id="ccbf7-112">address</span></span>|<span data-ttu-id="ccbf7-113">string</span><span class="sxs-lookup"><span data-stu-id="ccbf7-113">string</span></span>|<span data-ttu-id="ccbf7-114">Web サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="ccbf7-114">The URL of the website.</span></span>|
|<span data-ttu-id="ccbf7-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ccbf7-115">displayName</span></span>|<span data-ttu-id="ccbf7-116">string</span><span class="sxs-lookup"><span data-stu-id="ccbf7-116">string</span></span>|<span data-ttu-id="ccbf7-117">Web サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="ccbf7-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ccbf7-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ccbf7-118">JSON representation</span></span>

<span data-ttu-id="ccbf7-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ccbf7-119">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
