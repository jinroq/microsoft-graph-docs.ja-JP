---
title: educationOrganization リソースの種類
description: 教育セクター内の別の組織の種類との間の共通性をモデル化するために使用する抽象エンティティです。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 99f3294f76a246e4e78f0f61b0fc1f62532c3a03
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977424"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="6c2b6-103">educationOrganization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c2b6-103">educationOrganization resource type</span></span>

<span data-ttu-id="6c2b6-104">教育セクター内の別の組織の種類との間の共通性をモデル化するために使用する抽象エンティティです。</span><span class="sxs-lookup"><span data-stu-id="6c2b6-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="6c2b6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c2b6-105">Properties</span></span>
| <span data-ttu-id="6c2b6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c2b6-106">Property</span></span>     | <span data-ttu-id="6c2b6-107">種類</span><span class="sxs-lookup"><span data-stu-id="6c2b6-107">Type</span></span>   |<span data-ttu-id="6c2b6-108">説明</span><span class="sxs-lookup"><span data-stu-id="6c2b6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c2b6-109">説明</span><span class="sxs-lookup"><span data-stu-id="6c2b6-109">description</span></span>|<span data-ttu-id="6c2b6-110">String</span><span class="sxs-lookup"><span data-stu-id="6c2b6-110">String</span></span>| <span data-ttu-id="6c2b6-111">組織の説明です。</span><span class="sxs-lookup"><span data-stu-id="6c2b6-111">Organization description.</span></span>|
|<span data-ttu-id="6c2b6-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6c2b6-112">displayName</span></span>|<span data-ttu-id="6c2b6-113">String</span><span class="sxs-lookup"><span data-stu-id="6c2b6-113">String</span></span>| <span data-ttu-id="6c2b6-114">組織の表示名です。</span><span class="sxs-lookup"><span data-stu-id="6c2b6-114">Organization display name.</span></span>|
|<span data-ttu-id="6c2b6-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="6c2b6-115">externalSource</span></span>|<span data-ttu-id="6c2b6-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="6c2b6-116">educationExternalSource</span></span>| <span data-ttu-id="6c2b6-117">この組織が作成されたソースです。</span><span class="sxs-lookup"><span data-stu-id="6c2b6-117">Source where this organization was created from.</span></span> <span data-ttu-id="6c2b6-118">可能な値: `sis`、 `manual`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="6c2b6-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c2b6-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6c2b6-119">Relationships</span></span>
<span data-ttu-id="6c2b6-120">なし。</span><span class="sxs-lookup"><span data-stu-id="6c2b6-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6c2b6-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c2b6-121">JSON representation</span></span>

<span data-ttu-id="6c2b6-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6c2b6-122">The following is a JSON representation of the resource.</span></span>

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
