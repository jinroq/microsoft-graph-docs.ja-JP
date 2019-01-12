---
title: yammerActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d24e21c9525d49b7af5f8c4efaddd606c20c162b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923034"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="cf934-103">yammerActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cf934-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="cf934-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf934-104">Properties</span></span>

| <span data-ttu-id="cf934-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf934-105">Property</span></span>          | <span data-ttu-id="cf934-106">種類</span><span class="sxs-lookup"><span data-stu-id="cf934-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="cf934-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cf934-107">reportRefreshDate</span></span> | <span data-ttu-id="cf934-108">日付</span><span class="sxs-lookup"><span data-stu-id="cf934-108">Date</span></span>              |
| <span data-ttu-id="cf934-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cf934-109">userPrincipalName</span></span> | <span data-ttu-id="cf934-110">String</span><span class="sxs-lookup"><span data-stu-id="cf934-110">String</span></span>            |
| <span data-ttu-id="cf934-111">displayName</span><span class="sxs-lookup"><span data-stu-id="cf934-111">displayName</span></span>       | <span data-ttu-id="cf934-112">String</span><span class="sxs-lookup"><span data-stu-id="cf934-112">String</span></span>            |
| <span data-ttu-id="cf934-113">userState</span><span class="sxs-lookup"><span data-stu-id="cf934-113">userState</span></span>         | <span data-ttu-id="cf934-114">String</span><span class="sxs-lookup"><span data-stu-id="cf934-114">String</span></span>            |
| <span data-ttu-id="cf934-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="cf934-115">stateChangeDate</span></span>   | <span data-ttu-id="cf934-116">日付</span><span class="sxs-lookup"><span data-stu-id="cf934-116">Date</span></span>              |
| <span data-ttu-id="cf934-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="cf934-117">lastActivityDate</span></span>  | <span data-ttu-id="cf934-118">日付</span><span class="sxs-lookup"><span data-stu-id="cf934-118">Date</span></span>              |
| <span data-ttu-id="cf934-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="cf934-119">postedCount</span></span>       | <span data-ttu-id="cf934-120">Int64</span><span class="sxs-lookup"><span data-stu-id="cf934-120">Int64</span></span>             |
| <span data-ttu-id="cf934-121">readCount</span><span class="sxs-lookup"><span data-stu-id="cf934-121">readCount</span></span>         | <span data-ttu-id="cf934-122">Int64</span><span class="sxs-lookup"><span data-stu-id="cf934-122">Int64</span></span>             |
| <span data-ttu-id="cf934-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="cf934-123">likedCount</span></span>        | <span data-ttu-id="cf934-124">Int64</span><span class="sxs-lookup"><span data-stu-id="cf934-124">Int64</span></span>             |
| <span data-ttu-id="cf934-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="cf934-125">assignedProducts</span></span>  | <span data-ttu-id="cf934-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="cf934-126">String collection</span></span> |
| <span data-ttu-id="cf934-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cf934-127">reportPeriod</span></span>      | <span data-ttu-id="cf934-128">String</span><span class="sxs-lookup"><span data-stu-id="cf934-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="cf934-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cf934-129">JSON representation</span></span>

<span data-ttu-id="cf934-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cf934-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
