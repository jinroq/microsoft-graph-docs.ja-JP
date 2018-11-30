---
title: Web サイトのリソースの種類
description: Web サイトを表します。
ms.openlocfilehash: fa117dc6279e90b49c3c54d0a0ac534e30e633af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071976"
---
# <a name="website-resource-type"></a><span data-ttu-id="362b6-103">Web サイトのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="362b6-103">website resource type</span></span>

> <span data-ttu-id="362b6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="362b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="362b6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="362b6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="362b6-106">Web サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="362b6-106">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="362b6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="362b6-107">Properties</span></span>
| <span data-ttu-id="362b6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="362b6-108">Property</span></span>     | <span data-ttu-id="362b6-109">型</span><span class="sxs-lookup"><span data-stu-id="362b6-109">Type</span></span>   |<span data-ttu-id="362b6-110">説明</span><span class="sxs-lookup"><span data-stu-id="362b6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="362b6-111">type</span><span class="sxs-lookup"><span data-stu-id="362b6-111">type</span></span>|<span data-ttu-id="362b6-112">String</span><span class="sxs-lookup"><span data-stu-id="362b6-112">String</span></span>| <span data-ttu-id="362b6-113">可能な値は、`other`、`home`、`work`、`blog`、`profile` です。</span><span class="sxs-lookup"><span data-stu-id="362b6-113">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="362b6-114">アドレス</span><span class="sxs-lookup"><span data-stu-id="362b6-114">address</span></span>|<span data-ttu-id="362b6-115">文字列</span><span class="sxs-lookup"><span data-stu-id="362b6-115">string</span></span>|<span data-ttu-id="362b6-116">Web サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="362b6-116">The URL of the website.</span></span>|
|<span data-ttu-id="362b6-117">displayName</span><span class="sxs-lookup"><span data-stu-id="362b6-117">displayName</span></span>|<span data-ttu-id="362b6-118">string</span><span class="sxs-lookup"><span data-stu-id="362b6-118">string</span></span>|<span data-ttu-id="362b6-119">Web サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="362b6-119">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="362b6-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="362b6-120">JSON representation</span></span>

<span data-ttu-id="362b6-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="362b6-121">Here is a JSON representation of the resource.</span></span>

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