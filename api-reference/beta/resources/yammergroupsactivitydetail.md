---
title: yammerGroupsActivityDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c5b580f643686c27497fd24a6fe00c7750a6a938
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551422"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="31dba-103">yammerGroupsActivityDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31dba-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="31dba-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31dba-104">Properties</span></span>

| <span data-ttu-id="31dba-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31dba-105">Property</span></span>           | <span data-ttu-id="31dba-106">型</span><span class="sxs-lookup"><span data-stu-id="31dba-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="31dba-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="31dba-107">reportRefreshDate</span></span>  | <span data-ttu-id="31dba-108">Date</span><span class="sxs-lookup"><span data-stu-id="31dba-108">Date</span></span>    |
| <span data-ttu-id="31dba-109">groupdisplayname</span><span class="sxs-lookup"><span data-stu-id="31dba-109">groupDisplayName</span></span>   | <span data-ttu-id="31dba-110">String</span><span class="sxs-lookup"><span data-stu-id="31dba-110">String</span></span>  |
| <span data-ttu-id="31dba-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="31dba-111">isDeleted</span></span>          | <span data-ttu-id="31dba-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="31dba-112">Boolean</span></span> |
| <span data-ttu-id="31dba-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="31dba-113">ownerPrincipalName</span></span> | <span data-ttu-id="31dba-114">String</span><span class="sxs-lookup"><span data-stu-id="31dba-114">String</span></span>  |
| <span data-ttu-id="31dba-115">lastactivitydate</span><span class="sxs-lookup"><span data-stu-id="31dba-115">lastActivityDate</span></span>   | <span data-ttu-id="31dba-116">Date</span><span class="sxs-lookup"><span data-stu-id="31dba-116">Date</span></span>    |
| <span data-ttu-id="31dba-117">groupType</span><span class="sxs-lookup"><span data-stu-id="31dba-117">groupType</span></span>          | <span data-ttu-id="31dba-118">String</span><span class="sxs-lookup"><span data-stu-id="31dba-118">String</span></span>  |
| <span data-ttu-id="31dba-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="31dba-119">office365Connected</span></span> | <span data-ttu-id="31dba-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="31dba-120">Boolean</span></span> |
| <span data-ttu-id="31dba-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="31dba-121">memberCount</span></span>        | <span data-ttu-id="31dba-122">Int64</span><span class="sxs-lookup"><span data-stu-id="31dba-122">Int64</span></span>   |
| <span data-ttu-id="31dba-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="31dba-123">postedCount</span></span>        | <span data-ttu-id="31dba-124">Int64</span><span class="sxs-lookup"><span data-stu-id="31dba-124">Int64</span></span>   |
| <span data-ttu-id="31dba-125">readcount</span><span class="sxs-lookup"><span data-stu-id="31dba-125">readCount</span></span>          | <span data-ttu-id="31dba-126">Int64</span><span class="sxs-lookup"><span data-stu-id="31dba-126">Int64</span></span>   |
| <span data-ttu-id="31dba-127">dcount</span><span class="sxs-lookup"><span data-stu-id="31dba-127">likedCount</span></span>         | <span data-ttu-id="31dba-128">Int64</span><span class="sxs-lookup"><span data-stu-id="31dba-128">Int64</span></span>   |
| <span data-ttu-id="31dba-129">reportperiod</span><span class="sxs-lookup"><span data-stu-id="31dba-129">reportPeriod</span></span>       | <span data-ttu-id="31dba-130">String</span><span class="sxs-lookup"><span data-stu-id="31dba-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="31dba-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31dba-131">JSON representation</span></span>

<span data-ttu-id="31dba-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="31dba-132">The following is a JSON representation of the resource.</span></span>

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
