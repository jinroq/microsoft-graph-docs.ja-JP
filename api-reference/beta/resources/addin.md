---
title: アドイン リソースの種類
description: 以下は、リソースの JSON 表記です。
ms.openlocfilehash: c95f6bcc7fa26d77bc5a9595a6c80d0c4a94769c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072140"
---
# <a name="addin-resource-type"></a><span data-ttu-id="84c7e-103">アドイン リソースの種類</span><span class="sxs-lookup"><span data-stu-id="84c7e-103">addIn resource type</span></span>

> <span data-ttu-id="84c7e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="84c7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84c7e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84c7e-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="84c7e-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="84c7e-106">JSON representation</span></span>

<span data-ttu-id="84c7e-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="84c7e-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="84c7e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84c7e-108">Properties</span></span>
| <span data-ttu-id="84c7e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84c7e-109">Property</span></span>     | <span data-ttu-id="84c7e-110">型</span><span class="sxs-lookup"><span data-stu-id="84c7e-110">Type</span></span>   |<span data-ttu-id="84c7e-111">説明</span><span class="sxs-lookup"><span data-stu-id="84c7e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84c7e-112">ID</span><span class="sxs-lookup"><span data-stu-id="84c7e-112">id</span></span>|<span data-ttu-id="84c7e-113">guid</span><span class="sxs-lookup"><span data-stu-id="84c7e-113">guid</span></span>||
|<span data-ttu-id="84c7e-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84c7e-114">properties</span></span>|<span data-ttu-id="84c7e-115">[keyValue](keyvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="84c7e-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="84c7e-116">type</span><span class="sxs-lookup"><span data-stu-id="84c7e-116">type</span></span>|<span data-ttu-id="84c7e-117">文字列</span><span class="sxs-lookup"><span data-stu-id="84c7e-117">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->