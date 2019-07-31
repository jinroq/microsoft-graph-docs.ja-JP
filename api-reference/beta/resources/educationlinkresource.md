---
title: educationLinkResource リソースの種類
description: EducationResource のサブクラス。 このリソースはリンクであり、それに関連付けられている追加のデータはありません。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 58558ba55846614ce0bf0d08614faab34e4989af
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972657"
---
# <a name="educationlinkresource-resource-type"></a><span data-ttu-id="7f687-104">educationLinkResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f687-104">educationLinkResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f687-105">[EducationResource](educationresource.md)のサブクラス。</span><span class="sxs-lookup"><span data-stu-id="7f687-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="7f687-106">このリソースはリンクであり、それに関連付けられている追加のデータはありません。</span><span class="sxs-lookup"><span data-stu-id="7f687-106">This resource is a link and does not have any additional data associated with it.</span></span>


## <a name="properties"></a><span data-ttu-id="7f687-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f687-107">Properties</span></span>
| <span data-ttu-id="7f687-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f687-108">Property</span></span>     | <span data-ttu-id="7f687-109">型</span><span class="sxs-lookup"><span data-stu-id="7f687-109">Type</span></span>   |<span data-ttu-id="7f687-110">説明</span><span class="sxs-lookup"><span data-stu-id="7f687-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f687-111">link</span><span class="sxs-lookup"><span data-stu-id="7f687-111">link</span></span>|<span data-ttu-id="7f687-112">String</span><span class="sxs-lookup"><span data-stu-id="7f687-112">String</span></span>|<span data-ttu-id="7f687-113">リソースへの URL。</span><span class="sxs-lookup"><span data-stu-id="7f687-113">URL to the resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f687-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f687-114">JSON representation</span></span>

<span data-ttu-id="7f687-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f687-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
