---
title: Web サイトのリソースの種類
description: Web サイトを表します。
ms.openlocfilehash: 14934aae418581f4c75c880be67bf51fd0bc293c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020744"
---
# <a name="website-resource-type"></a><span data-ttu-id="2b112-103">Web サイトのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b112-103">website resource type</span></span>

<span data-ttu-id="2b112-104">Web サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="2b112-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="2b112-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b112-105">Properties</span></span>
| <span data-ttu-id="2b112-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b112-106">Property</span></span>     | <span data-ttu-id="2b112-107">型</span><span class="sxs-lookup"><span data-stu-id="2b112-107">Type</span></span>   |<span data-ttu-id="2b112-108">説明</span><span class="sxs-lookup"><span data-stu-id="2b112-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b112-109">type</span><span class="sxs-lookup"><span data-stu-id="2b112-109">type</span></span>|<span data-ttu-id="2b112-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="2b112-110">websiteType</span></span>| <span data-ttu-id="2b112-111">可能な値: `other`、 `home`、 `work`、 `blog`、 `profile`。</span><span class="sxs-lookup"><span data-stu-id="2b112-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="2b112-112">address</span><span class="sxs-lookup"><span data-stu-id="2b112-112">address</span></span>|<span data-ttu-id="2b112-113">文字列</span><span class="sxs-lookup"><span data-stu-id="2b112-113">string</span></span>|<span data-ttu-id="2b112-114">Web サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="2b112-114">The URL of the website.</span></span>|
|<span data-ttu-id="2b112-115">displayName</span><span class="sxs-lookup"><span data-stu-id="2b112-115">displayName</span></span>|<span data-ttu-id="2b112-116">string</span><span class="sxs-lookup"><span data-stu-id="2b112-116">string</span></span>|<span data-ttu-id="2b112-117">Web サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="2b112-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b112-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b112-118">JSON representation</span></span>

<span data-ttu-id="2b112-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b112-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
