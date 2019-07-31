---
title: educationOrganization リソースの種類
description: '教育機関内の異なる組織の種類間で共通性をモデル化するために使用される抽象エンティティ。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a28577dca488cb11bc6c34c7c653e0db1ede3d4e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972622"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="1801d-103">educationOrganization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1801d-103">educationOrganization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1801d-104">教育機関内の異なる組織の種類間で共通性をモデル化するために使用される抽象エンティティ。</span><span class="sxs-lookup"><span data-stu-id="1801d-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="1801d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1801d-105">Properties</span></span>
| <span data-ttu-id="1801d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1801d-106">Property</span></span>     | <span data-ttu-id="1801d-107">型</span><span class="sxs-lookup"><span data-stu-id="1801d-107">Type</span></span>   |<span data-ttu-id="1801d-108">説明</span><span class="sxs-lookup"><span data-stu-id="1801d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1801d-109">description</span><span class="sxs-lookup"><span data-stu-id="1801d-109">description</span></span>|<span data-ttu-id="1801d-110">String</span><span class="sxs-lookup"><span data-stu-id="1801d-110">String</span></span>| <span data-ttu-id="1801d-111">組織の説明。</span><span class="sxs-lookup"><span data-stu-id="1801d-111">Organization description.</span></span>|
|<span data-ttu-id="1801d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1801d-112">displayName</span></span>|<span data-ttu-id="1801d-113">String</span><span class="sxs-lookup"><span data-stu-id="1801d-113">String</span></span>| <span data-ttu-id="1801d-114">組織の表示名。</span><span class="sxs-lookup"><span data-stu-id="1801d-114">Organization display name.</span></span>|
|<span data-ttu-id="1801d-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="1801d-115">externalSource</span></span>|<span data-ttu-id="1801d-116">string</span><span class="sxs-lookup"><span data-stu-id="1801d-116">string</span></span>| <span data-ttu-id="1801d-117">この組織の作成元のソース。</span><span class="sxs-lookup"><span data-stu-id="1801d-117">Source where this organization was created from.</span></span> <span data-ttu-id="1801d-118">可能な値は、`sis`、`manual`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="1801d-118">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1801d-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1801d-119">Relationships</span></span>
<span data-ttu-id="1801d-120">なし。</span><span class="sxs-lookup"><span data-stu-id="1801d-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="1801d-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1801d-121">JSON representation</span></span>

<span data-ttu-id="1801d-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1801d-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
