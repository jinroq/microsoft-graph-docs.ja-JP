---
title: emailActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 16512c3a8a4dab62d4a71406d6c33d52a5a9bc08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818004"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="c6430-103">emailActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c6430-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c6430-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6430-104">Properties</span></span>

| <span data-ttu-id="c6430-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6430-105">Property</span></span>          | <span data-ttu-id="c6430-106">種類</span><span class="sxs-lookup"><span data-stu-id="c6430-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="c6430-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c6430-107">reportRefreshDate</span></span> | <span data-ttu-id="c6430-108">日付</span><span class="sxs-lookup"><span data-stu-id="c6430-108">Date</span></span>              |
| <span data-ttu-id="c6430-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c6430-109">userPrincipalName</span></span> | <span data-ttu-id="c6430-110">String</span><span class="sxs-lookup"><span data-stu-id="c6430-110">String</span></span>            |
| <span data-ttu-id="c6430-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c6430-111">displayName</span></span>       | <span data-ttu-id="c6430-112">String</span><span class="sxs-lookup"><span data-stu-id="c6430-112">String</span></span>            |
| <span data-ttu-id="c6430-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c6430-113">isDeleted</span></span>         | <span data-ttu-id="c6430-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="c6430-114">Boolean</span></span>           |
| <span data-ttu-id="c6430-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="c6430-115">deletedDate</span></span>       | <span data-ttu-id="c6430-116">日付</span><span class="sxs-lookup"><span data-stu-id="c6430-116">Date</span></span>              |
| <span data-ttu-id="c6430-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c6430-117">lastActivityDate</span></span>  | <span data-ttu-id="c6430-118">日付</span><span class="sxs-lookup"><span data-stu-id="c6430-118">Date</span></span>              |
| <span data-ttu-id="c6430-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="c6430-119">sendCount</span></span>         | <span data-ttu-id="c6430-120">Int64</span><span class="sxs-lookup"><span data-stu-id="c6430-120">Int64</span></span>             |
| <span data-ttu-id="c6430-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="c6430-121">receiveCount</span></span>      | <span data-ttu-id="c6430-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c6430-122">Int64</span></span>             |
| <span data-ttu-id="c6430-123">readCount</span><span class="sxs-lookup"><span data-stu-id="c6430-123">readCount</span></span>         | <span data-ttu-id="c6430-124">Int64</span><span class="sxs-lookup"><span data-stu-id="c6430-124">Int64</span></span>             |
| <span data-ttu-id="c6430-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="c6430-125">assignedProducts</span></span>  | <span data-ttu-id="c6430-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c6430-126">String collection</span></span> |
| <span data-ttu-id="c6430-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c6430-127">reportPeriod</span></span>      | <span data-ttu-id="c6430-128">String</span><span class="sxs-lookup"><span data-stu-id="c6430-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="c6430-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c6430-129">JSON representation</span></span>

<span data-ttu-id="c6430-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c6430-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
