---
title: importstatusmodel リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: fc1b0271d941b2e91d5b7ecbede9222de34a715e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340055"
---
# <a name="importstatusmodel-resource-type"></a><span data-ttu-id="637e4-103">importstatusmodel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="637e4-103">importStatusModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="637e4-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="637e4-104">JSON representation</span></span>

<span data-ttu-id="637e4-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="637e4-105">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="637e4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="637e4-106">Properties</span></span>
| <span data-ttu-id="637e4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="637e4-107">Property</span></span>     | <span data-ttu-id="637e4-108">型</span><span class="sxs-lookup"><span data-stu-id="637e4-108">Type</span></span>   |<span data-ttu-id="637e4-109">説明</span><span class="sxs-lookup"><span data-stu-id="637e4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="637e4-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="637e4-110">createdDateTime</span></span>| <span data-ttu-id="637e4-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="637e4-111">DateTimeOffset</span></span> ||
|<span data-ttu-id="637e4-112">id</span><span class="sxs-lookup"><span data-stu-id="637e4-112">id</span></span>|<span data-ttu-id="637e4-113">string</span><span class="sxs-lookup"><span data-stu-id="637e4-113">string</span></span>||
|<span data-ttu-id="637e4-114">status</span><span class="sxs-lookup"><span data-stu-id="637e4-114">status</span></span>|<span data-ttu-id="637e4-115">string</span><span class="sxs-lookup"><span data-stu-id="637e4-115">string</span></span>||

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
