---
title: アドイン リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: 6e76b8f7981be5da9a2ac8437ff21d4a59dbbe73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884217"
---
# <a name="addin-resource-type"></a><span data-ttu-id="d927d-103">アドイン リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d927d-103">addIn resource type</span></span>

> <span data-ttu-id="d927d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d927d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d927d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d927d-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d927d-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d927d-106">JSON representation</span></span>

<span data-ttu-id="d927d-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d927d-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyvalue"}],
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="d927d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d927d-108">Properties</span></span>
| <span data-ttu-id="d927d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d927d-109">Property</span></span>     | <span data-ttu-id="d927d-110">種類</span><span class="sxs-lookup"><span data-stu-id="d927d-110">Type</span></span>   |<span data-ttu-id="d927d-111">説明</span><span class="sxs-lookup"><span data-stu-id="d927d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d927d-112">ID</span><span class="sxs-lookup"><span data-stu-id="d927d-112">id</span></span>|<span data-ttu-id="d927d-113">guid</span><span class="sxs-lookup"><span data-stu-id="d927d-113">guid</span></span>||
|<span data-ttu-id="d927d-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d927d-114">properties</span></span>|<span data-ttu-id="d927d-115">[keyValue](keyvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d927d-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="d927d-116">type</span><span class="sxs-lookup"><span data-stu-id="d927d-116">type</span></span>|<span data-ttu-id="d927d-117">文字列</span><span class="sxs-lookup"><span data-stu-id="d927d-117">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
