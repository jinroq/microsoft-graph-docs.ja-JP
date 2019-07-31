---
title: mailboxUsageStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6f4ee4b29c82102db96cd4d71718f7da449776b5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009840"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="4f012-103">mailboxUsageStorage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4f012-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4f012-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f012-104">Properties</span></span>

| <span data-ttu-id="4f012-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f012-105">Property</span></span>           | <span data-ttu-id="4f012-106">型</span><span class="sxs-lookup"><span data-stu-id="4f012-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="4f012-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4f012-107">reportRefreshDate</span></span>  | <span data-ttu-id="4f012-108">日付</span><span class="sxs-lookup"><span data-stu-id="4f012-108">Date</span></span>   |
| <span data-ttu-id="4f012-109">Storageused Inbytes</span><span class="sxs-lookup"><span data-stu-id="4f012-109">storageUsedInBytes</span></span> | <span data-ttu-id="4f012-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4f012-110">Int64</span></span>  |
| <span data-ttu-id="4f012-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="4f012-111">reportDate</span></span>         | <span data-ttu-id="4f012-112">日付</span><span class="sxs-lookup"><span data-stu-id="4f012-112">Date</span></span>   |
| <span data-ttu-id="4f012-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4f012-113">reportPeriod</span></span>       | <span data-ttu-id="4f012-114">String</span><span class="sxs-lookup"><span data-stu-id="4f012-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4f012-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4f012-115">JSON representation</span></span>

<span data-ttu-id="4f012-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f012-116">The following is a JSON representation of the resource.</span></span>

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
