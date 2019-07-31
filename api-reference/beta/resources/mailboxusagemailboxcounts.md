---
title: mailboxUsageMailboxCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: b9f336e3d23cd84f79af7092463383a030336e13
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009861"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="4f1ab-103">mailboxUsageMailboxCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4f1ab-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4f1ab-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f1ab-104">Properties</span></span>

| <span data-ttu-id="4f1ab-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f1ab-105">Property</span></span>          | <span data-ttu-id="4f1ab-106">型</span><span class="sxs-lookup"><span data-stu-id="4f1ab-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4f1ab-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4f1ab-107">reportRefreshDate</span></span> | <span data-ttu-id="4f1ab-108">日付</span><span class="sxs-lookup"><span data-stu-id="4f1ab-108">Date</span></span>   |
| <span data-ttu-id="4f1ab-109">total</span><span class="sxs-lookup"><span data-stu-id="4f1ab-109">total</span></span>             | <span data-ttu-id="4f1ab-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4f1ab-110">Int64</span></span>  |
| <span data-ttu-id="4f1ab-111">active</span><span class="sxs-lookup"><span data-stu-id="4f1ab-111">active</span></span>            | <span data-ttu-id="4f1ab-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4f1ab-112">Int64</span></span>  |
| <span data-ttu-id="4f1ab-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="4f1ab-113">reportDate</span></span>        | <span data-ttu-id="4f1ab-114">日付</span><span class="sxs-lookup"><span data-stu-id="4f1ab-114">Date</span></span>   |
| <span data-ttu-id="4f1ab-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4f1ab-115">reportPeriod</span></span>      | <span data-ttu-id="4f1ab-116">String</span><span class="sxs-lookup"><span data-stu-id="4f1ab-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4f1ab-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4f1ab-117">JSON representation</span></span>

<span data-ttu-id="4f1ab-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f1ab-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
