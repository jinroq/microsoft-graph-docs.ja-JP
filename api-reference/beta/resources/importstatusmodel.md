---
title: importStatusModel リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: 47dbcdc97d0b70a1f7240e39fa73527ff12fae49
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882937"
---
# <a name="importstatusmodel-resource-type"></a><span data-ttu-id="9c4d5-103">importStatusModel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9c4d5-103">importStatusModel resource type</span></span>

> <span data-ttu-id="9c4d5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9c4d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c4d5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c4d5-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c4d5-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9c4d5-106">JSON representation</span></span>

<span data-ttu-id="9c4d5-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9c4d5-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.importstatusmodel"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "string",
  "status": "string"
}

```
## <a name="properties"></a><span data-ttu-id="9c4d5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c4d5-108">Properties</span></span>
| <span data-ttu-id="9c4d5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c4d5-109">Property</span></span>     | <span data-ttu-id="9c4d5-110">種類</span><span class="sxs-lookup"><span data-stu-id="9c4d5-110">Type</span></span>   |<span data-ttu-id="9c4d5-111">説明</span><span class="sxs-lookup"><span data-stu-id="9c4d5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c4d5-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c4d5-112">createdDateTime</span></span>| <span data-ttu-id="9c4d5-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c4d5-113">DateTimeOffset</span></span> ||
|<span data-ttu-id="9c4d5-114">ID</span><span class="sxs-lookup"><span data-stu-id="9c4d5-114">id</span></span>|<span data-ttu-id="9c4d5-115">文字列</span><span class="sxs-lookup"><span data-stu-id="9c4d5-115">string</span></span>||
|<span data-ttu-id="9c4d5-116">status</span><span class="sxs-lookup"><span data-stu-id="9c4d5-116">status</span></span>|<span data-ttu-id="9c4d5-117">文字列</span><span class="sxs-lookup"><span data-stu-id="9c4d5-117">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "importStatusModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
