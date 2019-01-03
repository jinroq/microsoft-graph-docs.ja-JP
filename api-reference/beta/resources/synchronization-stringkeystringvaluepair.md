---
title: stringKeyStringValuePair リソースの種類
description: キーが文字列、値は、文字列キーと値のペアを表します。
ms.openlocfilehash: 012625d78c8e07b3d38acba063acb57c751ced32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073528"
---
# <a name="stringkeystringvaluepair-resource-type"></a><span data-ttu-id="1db05-103">stringKeyStringValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1db05-103">stringKeyStringValuePair resource type</span></span>

> <span data-ttu-id="1db05-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1db05-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1db05-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1db05-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1db05-106">キーが文字列、値は、文字列キーと値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="1db05-106">Represents a key-value pair where the key is a string and the value is a string.</span></span>

## <a name="properties"></a><span data-ttu-id="1db05-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1db05-107">Properties</span></span>
| <span data-ttu-id="1db05-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1db05-108">Property</span></span>     | <span data-ttu-id="1db05-109">型</span><span class="sxs-lookup"><span data-stu-id="1db05-109">Type</span></span>   |<span data-ttu-id="1db05-110">説明</span><span class="sxs-lookup"><span data-stu-id="1db05-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1db05-111">Key</span><span class="sxs-lookup"><span data-stu-id="1db05-111">key</span></span>|<span data-ttu-id="1db05-112">String</span><span class="sxs-lookup"><span data-stu-id="1db05-112">String</span></span>|<span data-ttu-id="1db05-113">キー。</span><span class="sxs-lookup"><span data-stu-id="1db05-113">Key.</span></span>|
|<span data-ttu-id="1db05-114">value</span><span class="sxs-lookup"><span data-stu-id="1db05-114">value</span></span>|<span data-ttu-id="1db05-115">文字列</span><span class="sxs-lookup"><span data-stu-id="1db05-115">String</span></span>|<span data-ttu-id="1db05-116">値。</span><span class="sxs-lookup"><span data-stu-id="1db05-116">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1db05-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1db05-117">JSON representation</span></span>

<span data-ttu-id="1db05-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1db05-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->