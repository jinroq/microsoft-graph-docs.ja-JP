---
title: metadataEntry リソースの種類
description: 特定のオブジェクトのメタデータ。
localization_priority: Normal
ms.openlocfilehash: ffdb2dd3b6729320b5991b1158e10d145e339968
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819482"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="5e337-103">metadataEntry リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5e337-103">metadataEntry resource type</span></span>

> <span data-ttu-id="5e337-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5e337-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e337-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e337-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e337-106">特定のオブジェクトのメタデータ。</span><span class="sxs-lookup"><span data-stu-id="5e337-106">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="5e337-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e337-107">Properties</span></span>
| <span data-ttu-id="5e337-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e337-108">Property</span></span>     | <span data-ttu-id="5e337-109">種類</span><span class="sxs-lookup"><span data-stu-id="5e337-109">Type</span></span>   |<span data-ttu-id="5e337-110">説明</span><span class="sxs-lookup"><span data-stu-id="5e337-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e337-111">Key</span><span class="sxs-lookup"><span data-stu-id="5e337-111">key</span></span>|<span data-ttu-id="5e337-112">String</span><span class="sxs-lookup"><span data-stu-id="5e337-112">String</span></span>|<span data-ttu-id="5e337-113">メタデータ プロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="5e337-113">Name of the metadata property.</span></span>|
|<span data-ttu-id="5e337-114">value</span><span class="sxs-lookup"><span data-stu-id="5e337-114">value</span></span>|<span data-ttu-id="5e337-115">文字列</span><span class="sxs-lookup"><span data-stu-id="5e337-115">String</span></span>|<span data-ttu-id="5e337-116">メタデータ プロパティの値です。</span><span class="sxs-lookup"><span data-stu-id="5e337-116">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e337-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5e337-117">JSON representation</span></span>

<span data-ttu-id="5e337-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5e337-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
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
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
