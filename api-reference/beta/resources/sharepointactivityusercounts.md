---
title: sharePointActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: ffbbb8c4d33c94678e8d57d1d9e69da91b22fb39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819933"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="19cd0-103">sharePointActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="19cd0-103">sharePointActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="19cd0-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19cd0-104">Properties</span></span>

| <span data-ttu-id="19cd0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19cd0-105">Property</span></span>          | <span data-ttu-id="19cd0-106">種類</span><span class="sxs-lookup"><span data-stu-id="19cd0-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="19cd0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="19cd0-107">reportRefreshDate</span></span> | <span data-ttu-id="19cd0-108">日付</span><span class="sxs-lookup"><span data-stu-id="19cd0-108">Date</span></span>   |
| <span data-ttu-id="19cd0-109">visitedPage</span><span class="sxs-lookup"><span data-stu-id="19cd0-109">visitedPage</span></span>       | <span data-ttu-id="19cd0-110">Int64</span><span class="sxs-lookup"><span data-stu-id="19cd0-110">Int64</span></span>  |
| <span data-ttu-id="19cd0-111">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="19cd0-111">viewedOrEdited</span></span>    | <span data-ttu-id="19cd0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="19cd0-112">Int64</span></span>  |
| <span data-ttu-id="19cd0-113">同期</span><span class="sxs-lookup"><span data-stu-id="19cd0-113">synced</span></span>            | <span data-ttu-id="19cd0-114">Int64</span><span class="sxs-lookup"><span data-stu-id="19cd0-114">Int64</span></span>  |
| <span data-ttu-id="19cd0-115">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="19cd0-115">sharedInternally</span></span>  | <span data-ttu-id="19cd0-116">Int64</span><span class="sxs-lookup"><span data-stu-id="19cd0-116">Int64</span></span>  |
| <span data-ttu-id="19cd0-117">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="19cd0-117">sharedExternally</span></span>  | <span data-ttu-id="19cd0-118">Int64</span><span class="sxs-lookup"><span data-stu-id="19cd0-118">Int64</span></span>  |
| <span data-ttu-id="19cd0-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="19cd0-119">reportDate</span></span>        | <span data-ttu-id="19cd0-120">日付</span><span class="sxs-lookup"><span data-stu-id="19cd0-120">Date</span></span>   |
| <span data-ttu-id="19cd0-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="19cd0-121">reportPeriod</span></span>      | <span data-ttu-id="19cd0-122">String</span><span class="sxs-lookup"><span data-stu-id="19cd0-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="19cd0-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="19cd0-123">JSON representation</span></span>

<span data-ttu-id="19cd0-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19cd0-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPage": 1024, 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
