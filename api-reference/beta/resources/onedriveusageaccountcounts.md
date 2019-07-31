---
title: Onedrive のアカウント数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: bafc7ae26af6c94d61febb30c5a121f6f22ec7f0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009413"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="227e0-103">Onedrive のアカウント数リソースの種類</span><span class="sxs-lookup"><span data-stu-id="227e0-103">oneDriveUsageAccountCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="227e0-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="227e0-104">Properties</span></span>

| <span data-ttu-id="227e0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="227e0-105">Property</span></span>          | <span data-ttu-id="227e0-106">型</span><span class="sxs-lookup"><span data-stu-id="227e0-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="227e0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="227e0-107">reportRefreshDate</span></span> | <span data-ttu-id="227e0-108">日付</span><span class="sxs-lookup"><span data-stu-id="227e0-108">Date</span></span>   |
| <span data-ttu-id="227e0-109">siteType</span><span class="sxs-lookup"><span data-stu-id="227e0-109">siteType</span></span>          | <span data-ttu-id="227e0-110">String</span><span class="sxs-lookup"><span data-stu-id="227e0-110">String</span></span> |
| <span data-ttu-id="227e0-111">total</span><span class="sxs-lookup"><span data-stu-id="227e0-111">total</span></span>             | <span data-ttu-id="227e0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="227e0-112">Int64</span></span>  |
| <span data-ttu-id="227e0-113">active</span><span class="sxs-lookup"><span data-stu-id="227e0-113">active</span></span>            | <span data-ttu-id="227e0-114">Int64</span><span class="sxs-lookup"><span data-stu-id="227e0-114">Int64</span></span>  |
| <span data-ttu-id="227e0-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="227e0-115">reportDate</span></span>        | <span data-ttu-id="227e0-116">日付</span><span class="sxs-lookup"><span data-stu-id="227e0-116">Date</span></span>   |
| <span data-ttu-id="227e0-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="227e0-117">reportPeriod</span></span>      | <span data-ttu-id="227e0-118">String</span><span class="sxs-lookup"><span data-stu-id="227e0-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="227e0-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="227e0-119">JSON representation</span></span>

<span data-ttu-id="227e0-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="227e0-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
