---
title: yammerGroupsActivityDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: f16eda3f28556a18c47c68d532ace4244edfad19
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963753"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="0a765-103">yammerGroupsActivityDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a765-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0a765-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a765-104">Properties</span></span>

| <span data-ttu-id="0a765-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a765-105">Property</span></span>           | <span data-ttu-id="0a765-106">型</span><span class="sxs-lookup"><span data-stu-id="0a765-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="0a765-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0a765-107">reportRefreshDate</span></span>  | <span data-ttu-id="0a765-108">日付</span><span class="sxs-lookup"><span data-stu-id="0a765-108">Date</span></span>    |
| <span data-ttu-id="0a765-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="0a765-109">groupDisplayName</span></span>   | <span data-ttu-id="0a765-110">String</span><span class="sxs-lookup"><span data-stu-id="0a765-110">String</span></span>  |
| <span data-ttu-id="0a765-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="0a765-111">isDeleted</span></span>          | <span data-ttu-id="0a765-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a765-112">Boolean</span></span> |
| <span data-ttu-id="0a765-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0a765-113">ownerPrincipalName</span></span> | <span data-ttu-id="0a765-114">String</span><span class="sxs-lookup"><span data-stu-id="0a765-114">String</span></span>  |
| <span data-ttu-id="0a765-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="0a765-115">lastActivityDate</span></span>   | <span data-ttu-id="0a765-116">日付</span><span class="sxs-lookup"><span data-stu-id="0a765-116">Date</span></span>    |
| <span data-ttu-id="0a765-117">groupType</span><span class="sxs-lookup"><span data-stu-id="0a765-117">groupType</span></span>          | <span data-ttu-id="0a765-118">String</span><span class="sxs-lookup"><span data-stu-id="0a765-118">String</span></span>  |
| <span data-ttu-id="0a765-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="0a765-119">office365Connected</span></span> | <span data-ttu-id="0a765-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a765-120">Boolean</span></span> |
| <span data-ttu-id="0a765-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="0a765-121">memberCount</span></span>        | <span data-ttu-id="0a765-122">Int64</span><span class="sxs-lookup"><span data-stu-id="0a765-122">Int64</span></span>   |
| <span data-ttu-id="0a765-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="0a765-123">postedCount</span></span>        | <span data-ttu-id="0a765-124">Int64</span><span class="sxs-lookup"><span data-stu-id="0a765-124">Int64</span></span>   |
| <span data-ttu-id="0a765-125">readCount</span><span class="sxs-lookup"><span data-stu-id="0a765-125">readCount</span></span>          | <span data-ttu-id="0a765-126">Int64</span><span class="sxs-lookup"><span data-stu-id="0a765-126">Int64</span></span>   |
| <span data-ttu-id="0a765-127">Dcount</span><span class="sxs-lookup"><span data-stu-id="0a765-127">likedCount</span></span>         | <span data-ttu-id="0a765-128">Int64</span><span class="sxs-lookup"><span data-stu-id="0a765-128">Int64</span></span>   |
| <span data-ttu-id="0a765-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0a765-129">reportPeriod</span></span>       | <span data-ttu-id="0a765-130">String</span><span class="sxs-lookup"><span data-stu-id="0a765-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="0a765-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a765-131">JSON representation</span></span>

<span data-ttu-id="0a765-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0a765-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "office365Connected": true, 
  "memberCount": 1024, 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "reportPeriod": "String"
}
```
