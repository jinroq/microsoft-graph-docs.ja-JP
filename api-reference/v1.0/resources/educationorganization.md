---
title: educationOrganization リソースの種類
description: 教育機関内の異なる組織の種類間で共通性をモデル化するために使用される抽象エンティティ。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 99f3294f76a246e4e78f0f61b0fc1f62532c3a03
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562805"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="a23ea-103">educationOrganization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a23ea-103">educationOrganization resource type</span></span>

<span data-ttu-id="a23ea-104">教育機関内の異なる組織の種類間で共通性をモデル化するために使用される抽象エンティティ。</span><span class="sxs-lookup"><span data-stu-id="a23ea-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="a23ea-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a23ea-105">Properties</span></span>
| <span data-ttu-id="a23ea-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a23ea-106">Property</span></span>     | <span data-ttu-id="a23ea-107">型</span><span class="sxs-lookup"><span data-stu-id="a23ea-107">Type</span></span>   |<span data-ttu-id="a23ea-108">説明</span><span class="sxs-lookup"><span data-stu-id="a23ea-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a23ea-109">description</span><span class="sxs-lookup"><span data-stu-id="a23ea-109">description</span></span>|<span data-ttu-id="a23ea-110">String</span><span class="sxs-lookup"><span data-stu-id="a23ea-110">String</span></span>| <span data-ttu-id="a23ea-111">組織の説明。</span><span class="sxs-lookup"><span data-stu-id="a23ea-111">Organization description.</span></span>|
|<span data-ttu-id="a23ea-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a23ea-112">displayName</span></span>|<span data-ttu-id="a23ea-113">String</span><span class="sxs-lookup"><span data-stu-id="a23ea-113">String</span></span>| <span data-ttu-id="a23ea-114">組織の表示名。</span><span class="sxs-lookup"><span data-stu-id="a23ea-114">Organization display name.</span></span>|
|<span data-ttu-id="a23ea-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="a23ea-115">externalSource</span></span>|<span data-ttu-id="a23ea-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="a23ea-116">educationExternalSource</span></span>| <span data-ttu-id="a23ea-117">この組織の作成元のソース。</span><span class="sxs-lookup"><span data-stu-id="a23ea-117">Source where this organization was created from.</span></span> <span data-ttu-id="a23ea-118">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="a23ea-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a23ea-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a23ea-119">Relationships</span></span>
<span data-ttu-id="a23ea-120">なし。</span><span class="sxs-lookup"><span data-stu-id="a23ea-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a23ea-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a23ea-121">JSON representation</span></span>

<span data-ttu-id="a23ea-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a23ea-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
