---
title: office365ActivationsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0d5ed2af02f429f5fd4d6e92b408d2e8e420f4d0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574545"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="f32c8-103">office365ActivationsUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f32c8-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f32c8-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f32c8-104">Properties</span></span>

| <span data-ttu-id="f32c8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f32c8-105">Property</span></span>                 | <span data-ttu-id="f32c8-106">型</span><span class="sxs-lookup"><span data-stu-id="f32c8-106">Type</span></span>   | <span data-ttu-id="f32c8-107">説明</span><span class="sxs-lookup"><span data-stu-id="f32c8-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="f32c8-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f32c8-108">reportRefreshDate</span></span>        | <span data-ttu-id="f32c8-109">日付</span><span class="sxs-lookup"><span data-stu-id="f32c8-109">Date</span></span>   | <span data-ttu-id="f32c8-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="f32c8-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="f32c8-111">productType</span><span class="sxs-lookup"><span data-stu-id="f32c8-111">productType</span></span>              | <span data-ttu-id="f32c8-112">String</span><span class="sxs-lookup"><span data-stu-id="f32c8-112">String</span></span> | <span data-ttu-id="f32c8-113">「Office 365 用リソース"、「プロジェクト クライアント」などの製品の種類または"Office 365"の Visio Pro です。</span><span class="sxs-lookup"><span data-stu-id="f32c8-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="f32c8-114">割り当てられています。</span><span class="sxs-lookup"><span data-stu-id="f32c8-114">assigned</span></span>                 | <span data-ttu-id="f32c8-115">Int64</span><span class="sxs-lookup"><span data-stu-id="f32c8-115">Int64</span></span>  | <span data-ttu-id="f32c8-116">ユーザーの数は、製品のライセンスの割り当てられています。</span><span class="sxs-lookup"><span data-stu-id="f32c8-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="f32c8-117">アクティブ化</span><span class="sxs-lookup"><span data-stu-id="f32c8-117">activated</span></span>                | <span data-ttu-id="f32c8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f32c8-118">Int64</span></span>  | <span data-ttu-id="f32c8-119">製品をアクティブにしているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="f32c8-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="f32c8-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="f32c8-120">sharedComputerActivation</span></span> | <span data-ttu-id="f32c8-121">Int64</span><span class="sxs-lookup"><span data-stu-id="f32c8-121">Int64</span></span>  | <span data-ttu-id="f32c8-122">共有のコンピューターで製品を使用したユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="f32c8-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f32c8-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f32c8-123">JSON representation</span></span>

<span data-ttu-id="f32c8-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f32c8-124">The following is a JSON representation of the resource.</span></span>

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
