---
title: office365ActivationsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 33339578f498460aacd24481f166ab717138f8fa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966567"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="9f7a2-103">office365ActivationsUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f7a2-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9f7a2-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f7a2-104">Properties</span></span>

| <span data-ttu-id="9f7a2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f7a2-105">Property</span></span>                 | <span data-ttu-id="9f7a2-106">型</span><span class="sxs-lookup"><span data-stu-id="9f7a2-106">Type</span></span>   | <span data-ttu-id="9f7a2-107">説明</span><span class="sxs-lookup"><span data-stu-id="9f7a2-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="9f7a2-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9f7a2-108">reportRefreshDate</span></span>        | <span data-ttu-id="9f7a2-109">日付</span><span class="sxs-lookup"><span data-stu-id="9f7a2-109">Date</span></span>   | <span data-ttu-id="9f7a2-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="9f7a2-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="9f7a2-111">productType</span><span class="sxs-lookup"><span data-stu-id="9f7a2-111">productType</span></span>              | <span data-ttu-id="9f7a2-112">String</span><span class="sxs-lookup"><span data-stu-id="9f7a2-112">String</span></span> | <span data-ttu-id="9f7a2-113">"Office 365 ProPlus"、"Project Client"、または "Visio Pro for Office 365" などの製品の種類。</span><span class="sxs-lookup"><span data-stu-id="9f7a2-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="9f7a2-114">ら</span><span class="sxs-lookup"><span data-stu-id="9f7a2-114">assigned</span></span>                 | <span data-ttu-id="9f7a2-115">Int64</span><span class="sxs-lookup"><span data-stu-id="9f7a2-115">Int64</span></span>  | <span data-ttu-id="9f7a2-116">製品ライセンスに割り当てられているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="9f7a2-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="9f7a2-117">アクティブ化</span><span class="sxs-lookup"><span data-stu-id="9f7a2-117">activated</span></span>                | <span data-ttu-id="9f7a2-118">Int64</span><span class="sxs-lookup"><span data-stu-id="9f7a2-118">Int64</span></span>  | <span data-ttu-id="9f7a2-119">製品をライセンス認証したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="9f7a2-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="9f7a2-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="9f7a2-120">sharedComputerActivation</span></span> | <span data-ttu-id="9f7a2-121">Int64</span><span class="sxs-lookup"><span data-stu-id="9f7a2-121">Int64</span></span>  | <span data-ttu-id="9f7a2-122">共有コンピューターで製品を使用したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="9f7a2-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9f7a2-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f7a2-123">JSON representation</span></span>

<span data-ttu-id="9f7a2-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9f7a2-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```
