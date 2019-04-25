---
title: mailboxUsageStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 44b97c7b18264e01c86b34bfd8265246f80ab031
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524546"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="5f16a-103">mailboxUsageStorage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5f16a-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5f16a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f16a-104">Properties</span></span>

| <span data-ttu-id="5f16a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f16a-105">Property</span></span>           | <span data-ttu-id="5f16a-106">型</span><span class="sxs-lookup"><span data-stu-id="5f16a-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="5f16a-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="5f16a-107">reportRefreshDate</span></span>  | <span data-ttu-id="5f16a-108">Date</span><span class="sxs-lookup"><span data-stu-id="5f16a-108">Date</span></span>   |
| <span data-ttu-id="5f16a-109">storageused inbytes</span><span class="sxs-lookup"><span data-stu-id="5f16a-109">storageUsedInBytes</span></span> | <span data-ttu-id="5f16a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5f16a-110">Int64</span></span>  |
| <span data-ttu-id="5f16a-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="5f16a-111">reportDate</span></span>         | <span data-ttu-id="5f16a-112">Date</span><span class="sxs-lookup"><span data-stu-id="5f16a-112">Date</span></span>   |
| <span data-ttu-id="5f16a-113">reportperiod</span><span class="sxs-lookup"><span data-stu-id="5f16a-113">reportPeriod</span></span>       | <span data-ttu-id="5f16a-114">String</span><span class="sxs-lookup"><span data-stu-id="5f16a-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5f16a-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5f16a-115">JSON representation</span></span>

<span data-ttu-id="5f16a-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5f16a-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
