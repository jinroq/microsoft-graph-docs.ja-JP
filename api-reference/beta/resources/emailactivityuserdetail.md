---
title: emailActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 4f74b4af41c44e41b07bae1a8421011bc5188efc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066471"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="a9f27-103">emailActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a9f27-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a9f27-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9f27-104">Properties</span></span>

| <span data-ttu-id="a9f27-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9f27-105">Property</span></span>          | <span data-ttu-id="a9f27-106">型</span><span class="sxs-lookup"><span data-stu-id="a9f27-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="a9f27-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a9f27-107">reportRefreshDate</span></span> | <span data-ttu-id="a9f27-108">Date</span><span class="sxs-lookup"><span data-stu-id="a9f27-108">Date</span></span>              |
| <span data-ttu-id="a9f27-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9f27-109">userPrincipalName</span></span> | <span data-ttu-id="a9f27-110">String</span><span class="sxs-lookup"><span data-stu-id="a9f27-110">String</span></span>            |
| <span data-ttu-id="a9f27-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a9f27-111">displayName</span></span>       | <span data-ttu-id="a9f27-112">String</span><span class="sxs-lookup"><span data-stu-id="a9f27-112">String</span></span>            |
| <span data-ttu-id="a9f27-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a9f27-113">isDeleted</span></span>         | <span data-ttu-id="a9f27-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="a9f27-114">Boolean</span></span>           |
| <span data-ttu-id="a9f27-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="a9f27-115">deletedDate</span></span>       | <span data-ttu-id="a9f27-116">Date</span><span class="sxs-lookup"><span data-stu-id="a9f27-116">Date</span></span>              |
| <span data-ttu-id="a9f27-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a9f27-117">lastActivityDate</span></span>  | <span data-ttu-id="a9f27-118">Date</span><span class="sxs-lookup"><span data-stu-id="a9f27-118">Date</span></span>              |
| <span data-ttu-id="a9f27-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="a9f27-119">sendCount</span></span>         | <span data-ttu-id="a9f27-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a9f27-120">Int64</span></span>             |
| <span data-ttu-id="a9f27-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="a9f27-121">receiveCount</span></span>      | <span data-ttu-id="a9f27-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a9f27-122">Int64</span></span>             |
| <span data-ttu-id="a9f27-123">readCount</span><span class="sxs-lookup"><span data-stu-id="a9f27-123">readCount</span></span>         | <span data-ttu-id="a9f27-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a9f27-124">Int64</span></span>             |
| <span data-ttu-id="a9f27-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="a9f27-125">assignedProducts</span></span>  | <span data-ttu-id="a9f27-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a9f27-126">String collection</span></span> |
| <span data-ttu-id="a9f27-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a9f27-127">reportPeriod</span></span>      | <span data-ttu-id="a9f27-128">String</span><span class="sxs-lookup"><span data-stu-id="a9f27-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="a9f27-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a9f27-129">JSON representation</span></span>

<span data-ttu-id="a9f27-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a9f27-130">The following is a JSON representation of the resource.</span></span>

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
