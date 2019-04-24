---
title: educationOrganization リソースの種類
description: '教育機関内の異なる組織の種類間で共通性をモデル化するために使用される抽象エンティティ。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 122717952781cd8effe415fb01b07ec9bf71143d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507181"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="b1621-103">educationOrganization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b1621-103">educationOrganization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1621-104">教育機関内の異なる組織の種類間で共通性をモデル化するために使用される抽象エンティティ。</span><span class="sxs-lookup"><span data-stu-id="b1621-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="b1621-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1621-105">Properties</span></span>
| <span data-ttu-id="b1621-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1621-106">Property</span></span>     | <span data-ttu-id="b1621-107">型</span><span class="sxs-lookup"><span data-stu-id="b1621-107">Type</span></span>   |<span data-ttu-id="b1621-108">説明</span><span class="sxs-lookup"><span data-stu-id="b1621-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1621-109">description</span><span class="sxs-lookup"><span data-stu-id="b1621-109">description</span></span>|<span data-ttu-id="b1621-110">String</span><span class="sxs-lookup"><span data-stu-id="b1621-110">String</span></span>| <span data-ttu-id="b1621-111">組織の説明。</span><span class="sxs-lookup"><span data-stu-id="b1621-111">Organization description.</span></span>|
|<span data-ttu-id="b1621-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b1621-112">displayName</span></span>|<span data-ttu-id="b1621-113">String</span><span class="sxs-lookup"><span data-stu-id="b1621-113">String</span></span>| <span data-ttu-id="b1621-114">組織の表示名。</span><span class="sxs-lookup"><span data-stu-id="b1621-114">Organization display name.</span></span>|
|<span data-ttu-id="b1621-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="b1621-115">externalSource</span></span>|<span data-ttu-id="b1621-116">string</span><span class="sxs-lookup"><span data-stu-id="b1621-116">string</span></span>| <span data-ttu-id="b1621-117">この組織の作成元のソース。</span><span class="sxs-lookup"><span data-stu-id="b1621-117">Source where this organization was created from.</span></span> <span data-ttu-id="b1621-118">可能な値は、`sis`、`manual`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="b1621-118">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1621-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b1621-119">Relationships</span></span>
<span data-ttu-id="b1621-120">なし。</span><span class="sxs-lookup"><span data-stu-id="b1621-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b1621-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1621-121">JSON representation</span></span>

<span data-ttu-id="b1621-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b1621-122">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationorganization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
