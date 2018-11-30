---
title: yammerGroupsActivityDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 9a4bb00aecb2ae1d14b68a5388e0dedc7c41b1cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067444"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="a6140-103">yammerGroupsActivityDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a6140-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a6140-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6140-104">Properties</span></span>

| <span data-ttu-id="a6140-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6140-105">Property</span></span>           | <span data-ttu-id="a6140-106">型</span><span class="sxs-lookup"><span data-stu-id="a6140-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="a6140-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a6140-107">reportRefreshDate</span></span>  | <span data-ttu-id="a6140-108">Date</span><span class="sxs-lookup"><span data-stu-id="a6140-108">Date</span></span>    |
| <span data-ttu-id="a6140-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="a6140-109">groupDisplayName</span></span>   | <span data-ttu-id="a6140-110">String</span><span class="sxs-lookup"><span data-stu-id="a6140-110">String</span></span>  |
| <span data-ttu-id="a6140-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a6140-111">isDeleted</span></span>          | <span data-ttu-id="a6140-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="a6140-112">Boolean</span></span> |
| <span data-ttu-id="a6140-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a6140-113">ownerPrincipalName</span></span> | <span data-ttu-id="a6140-114">String</span><span class="sxs-lookup"><span data-stu-id="a6140-114">String</span></span>  |
| <span data-ttu-id="a6140-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a6140-115">lastActivityDate</span></span>   | <span data-ttu-id="a6140-116">Date</span><span class="sxs-lookup"><span data-stu-id="a6140-116">Date</span></span>    |
| <span data-ttu-id="a6140-117">groupType</span><span class="sxs-lookup"><span data-stu-id="a6140-117">groupType</span></span>          | <span data-ttu-id="a6140-118">String</span><span class="sxs-lookup"><span data-stu-id="a6140-118">String</span></span>  |
| <span data-ttu-id="a6140-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="a6140-119">office365Connected</span></span> | <span data-ttu-id="a6140-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="a6140-120">Boolean</span></span> |
| <span data-ttu-id="a6140-121">membercount プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6140-121">memberCount</span></span>        | <span data-ttu-id="a6140-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a6140-122">Int64</span></span>   |
| <span data-ttu-id="a6140-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="a6140-123">postedCount</span></span>        | <span data-ttu-id="a6140-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a6140-124">Int64</span></span>   |
| <span data-ttu-id="a6140-125">readCount</span><span class="sxs-lookup"><span data-stu-id="a6140-125">readCount</span></span>          | <span data-ttu-id="a6140-126">Int64</span><span class="sxs-lookup"><span data-stu-id="a6140-126">Int64</span></span>   |
| <span data-ttu-id="a6140-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="a6140-127">likedCount</span></span>         | <span data-ttu-id="a6140-128">Int64</span><span class="sxs-lookup"><span data-stu-id="a6140-128">Int64</span></span>   |
| <span data-ttu-id="a6140-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a6140-129">reportPeriod</span></span>       | <span data-ttu-id="a6140-130">String</span><span class="sxs-lookup"><span data-stu-id="a6140-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a6140-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6140-131">JSON representation</span></span>

<span data-ttu-id="a6140-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a6140-132">The following is a JSON representation of the resource.</span></span>

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
