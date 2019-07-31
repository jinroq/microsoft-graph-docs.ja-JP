---
title: yammerActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 960945d72db1cc347228983b9567968dfcfc52d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963788"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="97169-103">yammerActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97169-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="97169-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97169-104">Properties</span></span>

| <span data-ttu-id="97169-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97169-105">Property</span></span>          | <span data-ttu-id="97169-106">型</span><span class="sxs-lookup"><span data-stu-id="97169-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="97169-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="97169-107">reportRefreshDate</span></span> | <span data-ttu-id="97169-108">日付</span><span class="sxs-lookup"><span data-stu-id="97169-108">Date</span></span>              |
| <span data-ttu-id="97169-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="97169-109">userPrincipalName</span></span> | <span data-ttu-id="97169-110">String</span><span class="sxs-lookup"><span data-stu-id="97169-110">String</span></span>            |
| <span data-ttu-id="97169-111">displayName</span><span class="sxs-lookup"><span data-stu-id="97169-111">displayName</span></span>       | <span data-ttu-id="97169-112">文字列</span><span class="sxs-lookup"><span data-stu-id="97169-112">String</span></span>            |
| <span data-ttu-id="97169-113">userState</span><span class="sxs-lookup"><span data-stu-id="97169-113">userState</span></span>         | <span data-ttu-id="97169-114">String</span><span class="sxs-lookup"><span data-stu-id="97169-114">String</span></span>            |
| <span data-ttu-id="97169-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="97169-115">stateChangeDate</span></span>   | <span data-ttu-id="97169-116">日付</span><span class="sxs-lookup"><span data-stu-id="97169-116">Date</span></span>              |
| <span data-ttu-id="97169-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="97169-117">lastActivityDate</span></span>  | <span data-ttu-id="97169-118">日付</span><span class="sxs-lookup"><span data-stu-id="97169-118">Date</span></span>              |
| <span data-ttu-id="97169-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="97169-119">postedCount</span></span>       | <span data-ttu-id="97169-120">Int64</span><span class="sxs-lookup"><span data-stu-id="97169-120">Int64</span></span>             |
| <span data-ttu-id="97169-121">readCount</span><span class="sxs-lookup"><span data-stu-id="97169-121">readCount</span></span>         | <span data-ttu-id="97169-122">Int64</span><span class="sxs-lookup"><span data-stu-id="97169-122">Int64</span></span>             |
| <span data-ttu-id="97169-123">Dcount</span><span class="sxs-lookup"><span data-stu-id="97169-123">likedCount</span></span>        | <span data-ttu-id="97169-124">Int64</span><span class="sxs-lookup"><span data-stu-id="97169-124">Int64</span></span>             |
| <span data-ttu-id="97169-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="97169-125">assignedProducts</span></span>  | <span data-ttu-id="97169-126">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="97169-126">String collection</span></span> |
| <span data-ttu-id="97169-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="97169-127">reportPeriod</span></span>      | <span data-ttu-id="97169-128">String</span><span class="sxs-lookup"><span data-stu-id="97169-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="97169-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97169-129">JSON representation</span></span>

<span data-ttu-id="97169-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="97169-130">The following is a JSON representation of the resource.</span></span>

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
