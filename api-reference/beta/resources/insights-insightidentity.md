---
title: insightIdentity
description: 共有アイテムのプロパティを含む複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 8718ab248dada75f04d92d6a8717dd4f43ee8106
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333597"
---
# <a name="insightidentity"></a><span data-ttu-id="1ca4f-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="1ca4f-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ca4f-104">[共有](insights-shared.md)アイテムのプロパティを含む複合型。</span><span class="sxs-lookup"><span data-stu-id="1ca4f-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="1ca4f-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1ca4f-105">JSON representation</span></span>
<span data-ttu-id="1ca4f-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1ca4f-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="1ca4f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ca4f-107">Properties</span></span>

| <span data-ttu-id="1ca4f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ca4f-108">Property</span></span>              | <span data-ttu-id="1ca4f-109">型</span><span class="sxs-lookup"><span data-stu-id="1ca4f-109">Type</span></span>          | <span data-ttu-id="1ca4f-110">説明</span><span class="sxs-lookup"><span data-stu-id="1ca4f-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="1ca4f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1ca4f-111">displayName</span></span>       | <span data-ttu-id="1ca4f-112">String</span><span class="sxs-lookup"><span data-stu-id="1ca4f-112">String</span></span>          | <span data-ttu-id="1ca4f-113">アイテムを共有したユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="1ca4f-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="1ca4f-114">id</span><span class="sxs-lookup"><span data-stu-id="1ca4f-114">id</span></span>              | <span data-ttu-id="1ca4f-115">String</span><span class="sxs-lookup"><span data-stu-id="1ca4f-115">String</span></span>        | <span data-ttu-id="1ca4f-116">アイテムを共有したユーザーの id。</span><span class="sxs-lookup"><span data-stu-id="1ca4f-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="1ca4f-117">address</span><span class="sxs-lookup"><span data-stu-id="1ca4f-117">address</span></span>             | <span data-ttu-id="1ca4f-118">String</span><span class="sxs-lookup"><span data-stu-id="1ca4f-118">String</span></span>      | <span data-ttu-id="1ca4f-119">アイテムを共有したユーザーの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="1ca4f-119">The email address of the user who shared the item.</span></span>  |
