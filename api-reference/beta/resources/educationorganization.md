---
title: educationOrganization リソースの種類
description: '教育セクター内の別の組織の種類との間の共通性をモデル化するために使用する抽象エンティティです。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a1e3f82e2d777b1d32cc445f543e7beed570a8b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949522"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="e2ad7-103">educationOrganization リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e2ad7-103">educationOrganization resource type</span></span>

> <span data-ttu-id="e2ad7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e2ad7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2ad7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2ad7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2ad7-106">教育セクター内の別の組織の種類との間の共通性をモデル化するために使用する抽象エンティティです。</span><span class="sxs-lookup"><span data-stu-id="e2ad7-106">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="e2ad7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2ad7-107">Properties</span></span>
| <span data-ttu-id="e2ad7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2ad7-108">Property</span></span>     | <span data-ttu-id="e2ad7-109">種類</span><span class="sxs-lookup"><span data-stu-id="e2ad7-109">Type</span></span>   |<span data-ttu-id="e2ad7-110">説明</span><span class="sxs-lookup"><span data-stu-id="e2ad7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2ad7-111">説明</span><span class="sxs-lookup"><span data-stu-id="e2ad7-111">description</span></span>|<span data-ttu-id="e2ad7-112">String</span><span class="sxs-lookup"><span data-stu-id="e2ad7-112">String</span></span>| <span data-ttu-id="e2ad7-113">組織の説明です。</span><span class="sxs-lookup"><span data-stu-id="e2ad7-113">Organization description.</span></span>|
|<span data-ttu-id="e2ad7-114">displayName</span><span class="sxs-lookup"><span data-stu-id="e2ad7-114">displayName</span></span>|<span data-ttu-id="e2ad7-115">String</span><span class="sxs-lookup"><span data-stu-id="e2ad7-115">String</span></span>| <span data-ttu-id="e2ad7-116">組織の表示名です。</span><span class="sxs-lookup"><span data-stu-id="e2ad7-116">Organization display name.</span></span>|
|<span data-ttu-id="e2ad7-117">externalSource</span><span class="sxs-lookup"><span data-stu-id="e2ad7-117">externalSource</span></span>|<span data-ttu-id="e2ad7-118">文字列</span><span class="sxs-lookup"><span data-stu-id="e2ad7-118">string</span></span>| <span data-ttu-id="e2ad7-119">この組織が作成されたソースです。</span><span class="sxs-lookup"><span data-stu-id="e2ad7-119">Source where this organization was created from.</span></span> <span data-ttu-id="e2ad7-120">可能な値は、`sis`、`manual`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="e2ad7-120">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2ad7-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e2ad7-121">Relationships</span></span>
<span data-ttu-id="e2ad7-122">なし。</span><span class="sxs-lookup"><span data-stu-id="e2ad7-122">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e2ad7-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2ad7-123">JSON representation</span></span>

<span data-ttu-id="e2ad7-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2ad7-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
