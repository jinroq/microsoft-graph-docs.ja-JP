---
title: emailActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 039592a33cd004b9a5dc7800c0dbd4ece91bd48c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071884"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="66db4-103">emailActivitySummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66db4-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="66db4-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66db4-104">Properties</span></span>

| <span data-ttu-id="66db4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66db4-105">Property</span></span>          | <span data-ttu-id="66db4-106">型</span><span class="sxs-lookup"><span data-stu-id="66db4-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="66db4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="66db4-107">reportRefreshDate</span></span> | <span data-ttu-id="66db4-108">Date</span><span class="sxs-lookup"><span data-stu-id="66db4-108">Date</span></span>   |
| <span data-ttu-id="66db4-109">送信</span><span class="sxs-lookup"><span data-stu-id="66db4-109">send</span></span>              | <span data-ttu-id="66db4-110">Int64</span><span class="sxs-lookup"><span data-stu-id="66db4-110">Int64</span></span>  |
| <span data-ttu-id="66db4-111">表示されます。</span><span class="sxs-lookup"><span data-stu-id="66db4-111">receive</span></span>           | <span data-ttu-id="66db4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="66db4-112">Int64</span></span>  |
| <span data-ttu-id="66db4-113">読み取り</span><span class="sxs-lookup"><span data-stu-id="66db4-113">read</span></span>              | <span data-ttu-id="66db4-114">Int64</span><span class="sxs-lookup"><span data-stu-id="66db4-114">Int64</span></span>  |
| <span data-ttu-id="66db4-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="66db4-115">reportDate</span></span>        | <span data-ttu-id="66db4-116">Date</span><span class="sxs-lookup"><span data-stu-id="66db4-116">Date</span></span>   |
| <span data-ttu-id="66db4-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="66db4-117">reportPeriod</span></span>      | <span data-ttu-id="66db4-118">String</span><span class="sxs-lookup"><span data-stu-id="66db4-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66db4-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66db4-119">JSON representation</span></span>

<span data-ttu-id="66db4-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="66db4-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
