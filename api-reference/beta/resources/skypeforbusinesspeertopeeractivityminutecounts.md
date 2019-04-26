---
title: skypeForBusinessPeerToPeerActivityMinuteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 695c2fc57ab9d105b2576a9228ccc58d74b0094d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568153"
---
# <a name="skypeforbusinesspeertopeeractivityminutecounts-resource-type"></a><span data-ttu-id="f0218-103">skypeForBusinessPeerToPeerActivityMinuteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f0218-103">skypeForBusinessPeerToPeerActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f0218-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0218-104">Properties</span></span>

| <span data-ttu-id="f0218-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0218-105">Property</span></span>          | <span data-ttu-id="f0218-106">型</span><span class="sxs-lookup"><span data-stu-id="f0218-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f0218-107">audio</span><span class="sxs-lookup"><span data-stu-id="f0218-107">audio</span></span>             | <span data-ttu-id="f0218-108">Int64</span><span class="sxs-lookup"><span data-stu-id="f0218-108">Int64</span></span>  |
| <span data-ttu-id="f0218-109">video</span><span class="sxs-lookup"><span data-stu-id="f0218-109">video</span></span>             | <span data-ttu-id="f0218-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f0218-110">Int64</span></span>  |
| <span data-ttu-id="f0218-111">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="f0218-111">reportRefreshDate</span></span> | <span data-ttu-id="f0218-112">Date</span><span class="sxs-lookup"><span data-stu-id="f0218-112">Date</span></span>   |
| <span data-ttu-id="f0218-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="f0218-113">reportDate</span></span>        | <span data-ttu-id="f0218-114">Date</span><span class="sxs-lookup"><span data-stu-id="f0218-114">Date</span></span>   |
| <span data-ttu-id="f0218-115">reportperiod</span><span class="sxs-lookup"><span data-stu-id="f0218-115">reportPeriod</span></span>      | <span data-ttu-id="f0218-116">String</span><span class="sxs-lookup"><span data-stu-id="f0218-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f0218-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f0218-117">JSON representation</span></span>

<span data-ttu-id="f0218-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f0218-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```json
{
  "audio": 1024, 
  "video": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
