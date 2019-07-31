---
title: importStatusModel リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 917f83f005ba682d54722d51feea3f7ff872b0f5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973498"
---
# <a name="importstatusmodel-resource-type"></a><span data-ttu-id="748c1-103">importStatusModel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="748c1-103">importStatusModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="748c1-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="748c1-104">JSON representation</span></span>

<span data-ttu-id="748c1-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="748c1-105">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="748c1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="748c1-106">Properties</span></span>
| <span data-ttu-id="748c1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="748c1-107">Property</span></span>     | <span data-ttu-id="748c1-108">型</span><span class="sxs-lookup"><span data-stu-id="748c1-108">Type</span></span>   |<span data-ttu-id="748c1-109">説明</span><span class="sxs-lookup"><span data-stu-id="748c1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="748c1-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="748c1-110">createdDateTime</span></span>| <span data-ttu-id="748c1-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="748c1-111">DateTimeOffset</span></span> ||
|<span data-ttu-id="748c1-112">id</span><span class="sxs-lookup"><span data-stu-id="748c1-112">id</span></span>|<span data-ttu-id="748c1-113">string</span><span class="sxs-lookup"><span data-stu-id="748c1-113">string</span></span>||
|<span data-ttu-id="748c1-114">status</span><span class="sxs-lookup"><span data-stu-id="748c1-114">status</span></span>|<span data-ttu-id="748c1-115">string</span><span class="sxs-lookup"><span data-stu-id="748c1-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "importStatusModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
