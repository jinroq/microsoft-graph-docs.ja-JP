---
title: educationOrganization リソースの種類
description: 教育セクター内の別の組織の種類との間の共通性をモデル化するために使用する抽象エンティティです。
author: mmast-msft
ms.openlocfilehash: e4c0f69d63108cc88b88f530e99cbd55b23f49ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326146"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="8a547-103">educationOrganization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a547-103">educationOrganization resource type</span></span>

<span data-ttu-id="8a547-104">教育セクター内の別の組織の種類との間の共通性をモデル化するために使用する抽象エンティティです。</span><span class="sxs-lookup"><span data-stu-id="8a547-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="8a547-105">Properties</span><span class="sxs-lookup"><span data-stu-id="8a547-105">Properties</span></span>
| <span data-ttu-id="8a547-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a547-106">Property</span></span>     | <span data-ttu-id="8a547-107">種類</span><span class="sxs-lookup"><span data-stu-id="8a547-107">Type</span></span>   |<span data-ttu-id="8a547-108">説明</span><span class="sxs-lookup"><span data-stu-id="8a547-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a547-109">説明</span><span class="sxs-lookup"><span data-stu-id="8a547-109">description</span></span>|<span data-ttu-id="8a547-110">String</span><span class="sxs-lookup"><span data-stu-id="8a547-110">String</span></span>| <span data-ttu-id="8a547-111">組織の説明です。</span><span class="sxs-lookup"><span data-stu-id="8a547-111">Organization description.</span></span>|
|<span data-ttu-id="8a547-112">displayName</span><span class="sxs-lookup"><span data-stu-id="8a547-112">displayName</span></span>|<span data-ttu-id="8a547-113">String</span><span class="sxs-lookup"><span data-stu-id="8a547-113">String</span></span>| <span data-ttu-id="8a547-114">組織の表示名です。</span><span class="sxs-lookup"><span data-stu-id="8a547-114">Organization display name.</span></span>|
|<span data-ttu-id="8a547-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="8a547-115">externalSource</span></span>|<span data-ttu-id="8a547-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="8a547-116">educationExternalSource</span></span>| <span data-ttu-id="8a547-117">この組織が作成されたソースです。</span><span class="sxs-lookup"><span data-stu-id="8a547-117">Source where this organization was created from.</span></span> <span data-ttu-id="8a547-118">可能な値: `sis`、 `manual`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8a547-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a547-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a547-119">Relationships</span></span>
<span data-ttu-id="8a547-120">なし。</span><span class="sxs-lookup"><span data-stu-id="8a547-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8a547-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a547-121">JSON representation</span></span>

<span data-ttu-id="8a547-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8a547-122">The following is a JSON representation of the resource.</span></span>

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