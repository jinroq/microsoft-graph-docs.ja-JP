---
title: copystatusmodel リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: 1eb41726f2d72109ef4a297a1c994c9bae74fd5a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341042"
---
# <a name="copystatusmodel-resource-type"></a><span data-ttu-id="04e7e-103">copystatusmodel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="04e7e-103">copyStatusModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="04e7e-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="04e7e-104">JSON representation</span></span>

<span data-ttu-id="04e7e-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="04e7e-105">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="04e7e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04e7e-106">Properties</span></span>
| <span data-ttu-id="04e7e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04e7e-107">Property</span></span>     | <span data-ttu-id="04e7e-108">型</span><span class="sxs-lookup"><span data-stu-id="04e7e-108">Type</span></span>   |<span data-ttu-id="04e7e-109">説明</span><span class="sxs-lookup"><span data-stu-id="04e7e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04e7e-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04e7e-110">createdDateTime</span></span>| <span data-ttu-id="04e7e-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04e7e-111">DateTimeOffset</span></span> ||
|<span data-ttu-id="04e7e-112">id</span><span class="sxs-lookup"><span data-stu-id="04e7e-112">id</span></span>|<span data-ttu-id="04e7e-113">string</span><span class="sxs-lookup"><span data-stu-id="04e7e-113">string</span></span>||
|<span data-ttu-id="04e7e-114">status</span><span class="sxs-lookup"><span data-stu-id="04e7e-114">status</span></span>|<span data-ttu-id="04e7e-115">string</span><span class="sxs-lookup"><span data-stu-id="04e7e-115">string</span></span>||

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
