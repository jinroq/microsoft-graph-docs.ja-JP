---
title: skypeForBusinessActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2d723655e55c2702dd2b68adf65e43b6af16c36a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964936"
---
# <a name="skypeforbusinessactivityusercounts-resource-type"></a><span data-ttu-id="7f93c-103">skypeForBusinessActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f93c-103">skypeForBusinessActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7f93c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f93c-104">Properties</span></span>

| <span data-ttu-id="7f93c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f93c-105">Property</span></span>          | <span data-ttu-id="7f93c-106">型</span><span class="sxs-lookup"><span data-stu-id="7f93c-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7f93c-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="7f93c-107">peerToPeer</span></span>        | <span data-ttu-id="7f93c-108">Int64</span><span class="sxs-lookup"><span data-stu-id="7f93c-108">Int64</span></span>  |
| <span data-ttu-id="7f93c-109">別</span><span class="sxs-lookup"><span data-stu-id="7f93c-109">organized</span></span>         | <span data-ttu-id="7f93c-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7f93c-110">Int64</span></span>  |
| <span data-ttu-id="7f93c-111">参加した</span><span class="sxs-lookup"><span data-stu-id="7f93c-111">participated</span></span>      | <span data-ttu-id="7f93c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7f93c-112">Int64</span></span>  |
| <span data-ttu-id="7f93c-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7f93c-113">reportRefreshDate</span></span> | <span data-ttu-id="7f93c-114">日付</span><span class="sxs-lookup"><span data-stu-id="7f93c-114">Date</span></span>   |
| <span data-ttu-id="7f93c-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="7f93c-115">reportDate</span></span>        | <span data-ttu-id="7f93c-116">日付</span><span class="sxs-lookup"><span data-stu-id="7f93c-116">Date</span></span>   |
| <span data-ttu-id="7f93c-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7f93c-117">reportPeriod</span></span>      | <span data-ttu-id="7f93c-118">String</span><span class="sxs-lookup"><span data-stu-id="7f93c-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7f93c-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f93c-119">JSON representation</span></span>

<span data-ttu-id="7f93c-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f93c-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```json
{
  "peerToPeer": 1024, 
  "organized": 1024, 
  "participated": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
