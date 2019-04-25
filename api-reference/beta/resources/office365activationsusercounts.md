---
title: office365ActivationsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0d5ed2af02f429f5fd4d6e92b408d2e8e420f4d0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581514"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="6b198-103">office365ActivationsUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6b198-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6b198-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b198-104">Properties</span></span>

| <span data-ttu-id="6b198-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b198-105">Property</span></span>                 | <span data-ttu-id="6b198-106">型</span><span class="sxs-lookup"><span data-stu-id="6b198-106">Type</span></span>   | <span data-ttu-id="6b198-107">説明</span><span class="sxs-lookup"><span data-stu-id="6b198-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="6b198-108">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="6b198-108">reportRefreshDate</span></span>        | <span data-ttu-id="6b198-109">Date</span><span class="sxs-lookup"><span data-stu-id="6b198-109">Date</span></span>   | <span data-ttu-id="6b198-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="6b198-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="6b198-111">productType</span><span class="sxs-lookup"><span data-stu-id="6b198-111">productType</span></span>              | <span data-ttu-id="6b198-112">String</span><span class="sxs-lookup"><span data-stu-id="6b198-112">String</span></span> | <span data-ttu-id="6b198-113">"office 365 ProPlus"、"Project Client"、または "Visio Pro for Office 365" などの製品の種類。</span><span class="sxs-lookup"><span data-stu-id="6b198-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="6b198-114">ら</span><span class="sxs-lookup"><span data-stu-id="6b198-114">assigned</span></span>                 | <span data-ttu-id="6b198-115">Int64</span><span class="sxs-lookup"><span data-stu-id="6b198-115">Int64</span></span>  | <span data-ttu-id="6b198-116">製品ライセンスに割り当てられているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="6b198-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="6b198-117">アクティブ化</span><span class="sxs-lookup"><span data-stu-id="6b198-117">activated</span></span>                | <span data-ttu-id="6b198-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6b198-118">Int64</span></span>  | <span data-ttu-id="6b198-119">製品をライセンス認証したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="6b198-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="6b198-120">sharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="6b198-120">sharedComputerActivation</span></span> | <span data-ttu-id="6b198-121">Int64</span><span class="sxs-lookup"><span data-stu-id="6b198-121">Int64</span></span>  | <span data-ttu-id="6b198-122">共有コンピューターで製品を使用したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="6b198-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6b198-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6b198-123">JSON representation</span></span>

<span data-ttu-id="6b198-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6b198-124">The following is a JSON representation of the resource.</span></span>

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
