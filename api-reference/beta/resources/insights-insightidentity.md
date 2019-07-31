---
title: insightIdentity
description: 共有アイテムのプロパティを含む複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 6b5a4b3c6e43f0314860935af810d20d91663c96
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005752"
---
# <a name="insightidentity"></a><span data-ttu-id="6c1b4-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="6c1b4-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c1b4-104">[共有](insights-shared.md)アイテムのプロパティを含む複合型。</span><span class="sxs-lookup"><span data-stu-id="6c1b4-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="6c1b4-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c1b4-105">JSON representation</span></span>
<span data-ttu-id="6c1b4-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6c1b4-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="6c1b4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c1b4-107">Properties</span></span>

| <span data-ttu-id="6c1b4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c1b4-108">Property</span></span>              | <span data-ttu-id="6c1b4-109">型</span><span class="sxs-lookup"><span data-stu-id="6c1b4-109">Type</span></span>          | <span data-ttu-id="6c1b4-110">説明</span><span class="sxs-lookup"><span data-stu-id="6c1b4-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="6c1b4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6c1b4-111">displayName</span></span>       | <span data-ttu-id="6c1b4-112">String</span><span class="sxs-lookup"><span data-stu-id="6c1b4-112">String</span></span>          | <span data-ttu-id="6c1b4-113">アイテムを共有したユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="6c1b4-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="6c1b4-114">id</span><span class="sxs-lookup"><span data-stu-id="6c1b4-114">id</span></span>              | <span data-ttu-id="6c1b4-115">文字列</span><span class="sxs-lookup"><span data-stu-id="6c1b4-115">String</span></span>        | <span data-ttu-id="6c1b4-116">アイテムを共有したユーザーの id。</span><span class="sxs-lookup"><span data-stu-id="6c1b4-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="6c1b4-117">address</span><span class="sxs-lookup"><span data-stu-id="6c1b4-117">address</span></span>             | <span data-ttu-id="6c1b4-118">String</span><span class="sxs-lookup"><span data-stu-id="6c1b4-118">String</span></span>      | <span data-ttu-id="6c1b4-119">アイテムを共有したユーザーの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="6c1b4-119">The email address of the user who shared the item.</span></span>  |
