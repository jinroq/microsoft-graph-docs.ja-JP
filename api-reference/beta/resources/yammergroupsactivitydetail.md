---
title: yammerGroupsActivityDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 9e4ac61f2af69b4229c2e9c3df7c653428cc2033
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832033"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="046c4-103">yammerGroupsActivityDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="046c4-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="046c4-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="046c4-104">Properties</span></span>

| <span data-ttu-id="046c4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="046c4-105">Property</span></span>           | <span data-ttu-id="046c4-106">種類</span><span class="sxs-lookup"><span data-stu-id="046c4-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="046c4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="046c4-107">reportRefreshDate</span></span>  | <span data-ttu-id="046c4-108">日付</span><span class="sxs-lookup"><span data-stu-id="046c4-108">Date</span></span>    |
| <span data-ttu-id="046c4-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="046c4-109">groupDisplayName</span></span>   | <span data-ttu-id="046c4-110">String</span><span class="sxs-lookup"><span data-stu-id="046c4-110">String</span></span>  |
| <span data-ttu-id="046c4-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="046c4-111">isDeleted</span></span>          | <span data-ttu-id="046c4-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="046c4-112">Boolean</span></span> |
| <span data-ttu-id="046c4-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="046c4-113">ownerPrincipalName</span></span> | <span data-ttu-id="046c4-114">String</span><span class="sxs-lookup"><span data-stu-id="046c4-114">String</span></span>  |
| <span data-ttu-id="046c4-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="046c4-115">lastActivityDate</span></span>   | <span data-ttu-id="046c4-116">日付</span><span class="sxs-lookup"><span data-stu-id="046c4-116">Date</span></span>    |
| <span data-ttu-id="046c4-117">groupType</span><span class="sxs-lookup"><span data-stu-id="046c4-117">groupType</span></span>          | <span data-ttu-id="046c4-118">String</span><span class="sxs-lookup"><span data-stu-id="046c4-118">String</span></span>  |
| <span data-ttu-id="046c4-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="046c4-119">office365Connected</span></span> | <span data-ttu-id="046c4-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="046c4-120">Boolean</span></span> |
| <span data-ttu-id="046c4-121">membercount プロパティ</span><span class="sxs-lookup"><span data-stu-id="046c4-121">memberCount</span></span>        | <span data-ttu-id="046c4-122">Int64</span><span class="sxs-lookup"><span data-stu-id="046c4-122">Int64</span></span>   |
| <span data-ttu-id="046c4-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="046c4-123">postedCount</span></span>        | <span data-ttu-id="046c4-124">Int64</span><span class="sxs-lookup"><span data-stu-id="046c4-124">Int64</span></span>   |
| <span data-ttu-id="046c4-125">readCount</span><span class="sxs-lookup"><span data-stu-id="046c4-125">readCount</span></span>          | <span data-ttu-id="046c4-126">Int64</span><span class="sxs-lookup"><span data-stu-id="046c4-126">Int64</span></span>   |
| <span data-ttu-id="046c4-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="046c4-127">likedCount</span></span>         | <span data-ttu-id="046c4-128">Int64</span><span class="sxs-lookup"><span data-stu-id="046c4-128">Int64</span></span>   |
| <span data-ttu-id="046c4-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="046c4-129">reportPeriod</span></span>       | <span data-ttu-id="046c4-130">String</span><span class="sxs-lookup"><span data-stu-id="046c4-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="046c4-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="046c4-131">JSON representation</span></span>

<span data-ttu-id="046c4-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="046c4-132">The following is a JSON representation of the resource.</span></span>

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
