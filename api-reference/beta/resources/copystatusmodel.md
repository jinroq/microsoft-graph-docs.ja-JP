---
title: copyStatusModel リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2bc83b7eb519b3d11adc9f548becbec4444f1ef0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973969"
---
# <a name="copystatusmodel-resource-type"></a><span data-ttu-id="f6cd9-103">copyStatusModel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f6cd9-103">copyStatusModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="f6cd9-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f6cd9-104">JSON representation</span></span>

<span data-ttu-id="f6cd9-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f6cd9-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.copystatusmodel"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "string",
  "status": "string"
}

```
## <a name="properties"></a><span data-ttu-id="f6cd9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6cd9-106">Properties</span></span>
| <span data-ttu-id="f6cd9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6cd9-107">Property</span></span>     | <span data-ttu-id="f6cd9-108">型</span><span class="sxs-lookup"><span data-stu-id="f6cd9-108">Type</span></span>   |<span data-ttu-id="f6cd9-109">説明</span><span class="sxs-lookup"><span data-stu-id="f6cd9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6cd9-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6cd9-110">createdDateTime</span></span>| <span data-ttu-id="f6cd9-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6cd9-111">DateTimeOffset</span></span> ||
|<span data-ttu-id="f6cd9-112">id</span><span class="sxs-lookup"><span data-stu-id="f6cd9-112">id</span></span>|<span data-ttu-id="f6cd9-113">string</span><span class="sxs-lookup"><span data-stu-id="f6cd9-113">string</span></span>||
|<span data-ttu-id="f6cd9-114">status</span><span class="sxs-lookup"><span data-stu-id="f6cd9-114">status</span></span>|<span data-ttu-id="f6cd9-115">string</span><span class="sxs-lookup"><span data-stu-id="f6cd9-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "copyStatusModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
