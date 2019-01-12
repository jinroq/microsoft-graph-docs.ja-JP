---
title: yammerGroupsActivityDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 79ce924fff5d1ce9ca861c3d48589a0ecad149dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939169"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="b48b1-103">yammerGroupsActivityDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b48b1-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b48b1-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b48b1-104">Properties</span></span>

| <span data-ttu-id="b48b1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b48b1-105">Property</span></span>           | <span data-ttu-id="b48b1-106">種類</span><span class="sxs-lookup"><span data-stu-id="b48b1-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="b48b1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b48b1-107">reportRefreshDate</span></span>  | <span data-ttu-id="b48b1-108">日付</span><span class="sxs-lookup"><span data-stu-id="b48b1-108">Date</span></span>    |
| <span data-ttu-id="b48b1-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="b48b1-109">groupDisplayName</span></span>   | <span data-ttu-id="b48b1-110">String</span><span class="sxs-lookup"><span data-stu-id="b48b1-110">String</span></span>  |
| <span data-ttu-id="b48b1-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="b48b1-111">isDeleted</span></span>          | <span data-ttu-id="b48b1-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="b48b1-112">Boolean</span></span> |
| <span data-ttu-id="b48b1-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b48b1-113">ownerPrincipalName</span></span> | <span data-ttu-id="b48b1-114">String</span><span class="sxs-lookup"><span data-stu-id="b48b1-114">String</span></span>  |
| <span data-ttu-id="b48b1-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="b48b1-115">lastActivityDate</span></span>   | <span data-ttu-id="b48b1-116">日付</span><span class="sxs-lookup"><span data-stu-id="b48b1-116">Date</span></span>    |
| <span data-ttu-id="b48b1-117">groupType</span><span class="sxs-lookup"><span data-stu-id="b48b1-117">groupType</span></span>          | <span data-ttu-id="b48b1-118">String</span><span class="sxs-lookup"><span data-stu-id="b48b1-118">String</span></span>  |
| <span data-ttu-id="b48b1-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="b48b1-119">office365Connected</span></span> | <span data-ttu-id="b48b1-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="b48b1-120">Boolean</span></span> |
| <span data-ttu-id="b48b1-121">membercount プロパティ</span><span class="sxs-lookup"><span data-stu-id="b48b1-121">memberCount</span></span>        | <span data-ttu-id="b48b1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="b48b1-122">Int64</span></span>   |
| <span data-ttu-id="b48b1-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="b48b1-123">postedCount</span></span>        | <span data-ttu-id="b48b1-124">Int64</span><span class="sxs-lookup"><span data-stu-id="b48b1-124">Int64</span></span>   |
| <span data-ttu-id="b48b1-125">readCount</span><span class="sxs-lookup"><span data-stu-id="b48b1-125">readCount</span></span>          | <span data-ttu-id="b48b1-126">Int64</span><span class="sxs-lookup"><span data-stu-id="b48b1-126">Int64</span></span>   |
| <span data-ttu-id="b48b1-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="b48b1-127">likedCount</span></span>         | <span data-ttu-id="b48b1-128">Int64</span><span class="sxs-lookup"><span data-stu-id="b48b1-128">Int64</span></span>   |
| <span data-ttu-id="b48b1-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b48b1-129">reportPeriod</span></span>       | <span data-ttu-id="b48b1-130">String</span><span class="sxs-lookup"><span data-stu-id="b48b1-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="b48b1-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b48b1-131">JSON representation</span></span>

<span data-ttu-id="b48b1-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b48b1-132">The following is a JSON representation of the resource.</span></span>

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
