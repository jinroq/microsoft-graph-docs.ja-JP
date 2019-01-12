---
title: office365ActivationsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3dc497e516f95f1e05167703f2b9f8aea6363a64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917721"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="143d0-103">office365ActivationsUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="143d0-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="143d0-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="143d0-104">Properties</span></span>

| <span data-ttu-id="143d0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="143d0-105">Property</span></span>                 | <span data-ttu-id="143d0-106">種類</span><span class="sxs-lookup"><span data-stu-id="143d0-106">Type</span></span>   | <span data-ttu-id="143d0-107">説明</span><span class="sxs-lookup"><span data-stu-id="143d0-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="143d0-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="143d0-108">reportRefreshDate</span></span>        | <span data-ttu-id="143d0-109">日付</span><span class="sxs-lookup"><span data-stu-id="143d0-109">Date</span></span>   | <span data-ttu-id="143d0-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="143d0-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="143d0-111">productType</span><span class="sxs-lookup"><span data-stu-id="143d0-111">productType</span></span>              | <span data-ttu-id="143d0-112">String</span><span class="sxs-lookup"><span data-stu-id="143d0-112">String</span></span> | <span data-ttu-id="143d0-113">「Office 365 用リソース"、「プロジェクト クライアント」などの製品の種類または"Office 365"の Visio Pro です。</span><span class="sxs-lookup"><span data-stu-id="143d0-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="143d0-114">割り当てられています。</span><span class="sxs-lookup"><span data-stu-id="143d0-114">assigned</span></span>                 | <span data-ttu-id="143d0-115">Int64</span><span class="sxs-lookup"><span data-stu-id="143d0-115">Int64</span></span>  | <span data-ttu-id="143d0-116">ユーザーの数は、製品のライセンスの割り当てられています。</span><span class="sxs-lookup"><span data-stu-id="143d0-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="143d0-117">アクティブ化</span><span class="sxs-lookup"><span data-stu-id="143d0-117">activated</span></span>                | <span data-ttu-id="143d0-118">Int64</span><span class="sxs-lookup"><span data-stu-id="143d0-118">Int64</span></span>  | <span data-ttu-id="143d0-119">製品をアクティブにしているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="143d0-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="143d0-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="143d0-120">sharedComputerActivation</span></span> | <span data-ttu-id="143d0-121">Int64</span><span class="sxs-lookup"><span data-stu-id="143d0-121">Int64</span></span>  | <span data-ttu-id="143d0-122">共有のコンピューターで製品を使用したユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="143d0-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="143d0-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="143d0-123">JSON representation</span></span>

<span data-ttu-id="143d0-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="143d0-124">The following is a JSON representation of the resource.</span></span>

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
