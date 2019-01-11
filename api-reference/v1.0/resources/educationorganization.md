---
title: educationOrganization リソースの種類
description: 教育セクター内の別の組織の種類との間の共通性をモデル化するために使用する抽象エンティティです。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: b0b65978b3b415af407c886095c4b31c7aaffab9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831935"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="4b1ce-103">educationOrganization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b1ce-103">educationOrganization resource type</span></span>

<span data-ttu-id="4b1ce-104">教育セクター内の別の組織の種類との間の共通性をモデル化するために使用する抽象エンティティです。</span><span class="sxs-lookup"><span data-stu-id="4b1ce-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="4b1ce-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b1ce-105">Properties</span></span>
| <span data-ttu-id="4b1ce-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b1ce-106">Property</span></span>     | <span data-ttu-id="4b1ce-107">種類</span><span class="sxs-lookup"><span data-stu-id="4b1ce-107">Type</span></span>   |<span data-ttu-id="4b1ce-108">説明</span><span class="sxs-lookup"><span data-stu-id="4b1ce-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b1ce-109">説明</span><span class="sxs-lookup"><span data-stu-id="4b1ce-109">description</span></span>|<span data-ttu-id="4b1ce-110">String</span><span class="sxs-lookup"><span data-stu-id="4b1ce-110">String</span></span>| <span data-ttu-id="4b1ce-111">組織の説明です。</span><span class="sxs-lookup"><span data-stu-id="4b1ce-111">Organization description.</span></span>|
|<span data-ttu-id="4b1ce-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4b1ce-112">displayName</span></span>|<span data-ttu-id="4b1ce-113">String</span><span class="sxs-lookup"><span data-stu-id="4b1ce-113">String</span></span>| <span data-ttu-id="4b1ce-114">組織の表示名です。</span><span class="sxs-lookup"><span data-stu-id="4b1ce-114">Organization display name.</span></span>|
|<span data-ttu-id="4b1ce-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="4b1ce-115">externalSource</span></span>|<span data-ttu-id="4b1ce-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="4b1ce-116">educationExternalSource</span></span>| <span data-ttu-id="4b1ce-117">この組織が作成されたソースです。</span><span class="sxs-lookup"><span data-stu-id="4b1ce-117">Source where this organization was created from.</span></span> <span data-ttu-id="4b1ce-118">可能な値: `sis`、 `manual`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4b1ce-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b1ce-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4b1ce-119">Relationships</span></span>
<span data-ttu-id="4b1ce-120">なし。</span><span class="sxs-lookup"><span data-stu-id="4b1ce-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4b1ce-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b1ce-121">JSON representation</span></span>

<span data-ttu-id="4b1ce-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4b1ce-122">The following is a JSON representation of the resource.</span></span>

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
