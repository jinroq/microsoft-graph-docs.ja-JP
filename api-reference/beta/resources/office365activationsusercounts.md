---
title: office365ActivationsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 90d9d2d8616f166eb9d8b87967898daa0468db54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073072"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="dd5bd-103">office365ActivationsUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dd5bd-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="dd5bd-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd5bd-104">Properties</span></span>

| <span data-ttu-id="dd5bd-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd5bd-105">Property</span></span>                 | <span data-ttu-id="dd5bd-106">型</span><span class="sxs-lookup"><span data-stu-id="dd5bd-106">Type</span></span>   | <span data-ttu-id="dd5bd-107">説明</span><span class="sxs-lookup"><span data-stu-id="dd5bd-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="dd5bd-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="dd5bd-108">reportRefreshDate</span></span>        | <span data-ttu-id="dd5bd-109">Date</span><span class="sxs-lookup"><span data-stu-id="dd5bd-109">Date</span></span>   | <span data-ttu-id="dd5bd-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="dd5bd-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="dd5bd-111">productType</span><span class="sxs-lookup"><span data-stu-id="dd5bd-111">productType</span></span>              | <span data-ttu-id="dd5bd-112">String</span><span class="sxs-lookup"><span data-stu-id="dd5bd-112">String</span></span> | <span data-ttu-id="dd5bd-113">「Office 365 用リソース"、「プロジェクト クライアント」などの製品の種類または"Office 365"の Visio Pro です。</span><span class="sxs-lookup"><span data-stu-id="dd5bd-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="dd5bd-114">割り当てられています。</span><span class="sxs-lookup"><span data-stu-id="dd5bd-114">assigned</span></span>                 | <span data-ttu-id="dd5bd-115">Int64</span><span class="sxs-lookup"><span data-stu-id="dd5bd-115">Int64</span></span>  | <span data-ttu-id="dd5bd-116">ユーザーの数は、製品のライセンスの割り当てられています。</span><span class="sxs-lookup"><span data-stu-id="dd5bd-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="dd5bd-117">アクティブ化</span><span class="sxs-lookup"><span data-stu-id="dd5bd-117">activated</span></span>                | <span data-ttu-id="dd5bd-118">Int64</span><span class="sxs-lookup"><span data-stu-id="dd5bd-118">Int64</span></span>  | <span data-ttu-id="dd5bd-119">製品をアクティブにしているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="dd5bd-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="dd5bd-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="dd5bd-120">sharedComputerActivation</span></span> | <span data-ttu-id="dd5bd-121">Int64</span><span class="sxs-lookup"><span data-stu-id="dd5bd-121">Int64</span></span>  | <span data-ttu-id="dd5bd-122">共有のコンピューターで製品を使用したユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="dd5bd-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dd5bd-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dd5bd-123">JSON representation</span></span>

<span data-ttu-id="dd5bd-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dd5bd-124">The following is a JSON representation of the resource.</span></span>

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
