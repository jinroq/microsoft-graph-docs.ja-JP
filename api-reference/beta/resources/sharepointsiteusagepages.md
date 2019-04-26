---
title: sharepointsiteの pages リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1a82c0a1174559db6d90e64f1fd1ed1403caa048
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584055"
---
# <a name="sharepointsiteusagepages-resource-type"></a><span data-ttu-id="3905c-103">sharepointsiteの pages リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3905c-103">sharePointSiteUsagePages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3905c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3905c-104">Properties</span></span>

| <span data-ttu-id="3905c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3905c-105">Property</span></span>          | <span data-ttu-id="3905c-106">型</span><span class="sxs-lookup"><span data-stu-id="3905c-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="3905c-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="3905c-107">reportRefreshDate</span></span> | <span data-ttu-id="3905c-108">Date</span><span class="sxs-lookup"><span data-stu-id="3905c-108">Date</span></span>   |
| <span data-ttu-id="3905c-109">sitetype</span><span class="sxs-lookup"><span data-stu-id="3905c-109">siteType</span></span>          | <span data-ttu-id="3905c-110">String</span><span class="sxs-lookup"><span data-stu-id="3905c-110">String</span></span> |
| <span data-ttu-id="3905c-111">pageviewcount</span><span class="sxs-lookup"><span data-stu-id="3905c-111">pageViewCount</span></span>     | <span data-ttu-id="3905c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3905c-112">Int64</span></span>  |
| <span data-ttu-id="3905c-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="3905c-113">reportDate</span></span>        | <span data-ttu-id="3905c-114">Date</span><span class="sxs-lookup"><span data-stu-id="3905c-114">Date</span></span>   |
| <span data-ttu-id="3905c-115">reportperiod</span><span class="sxs-lookup"><span data-stu-id="3905c-115">reportPeriod</span></span>      | <span data-ttu-id="3905c-116">String</span><span class="sxs-lookup"><span data-stu-id="3905c-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3905c-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3905c-117">JSON representation</span></span>

<span data-ttu-id="3905c-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3905c-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsagePages"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "pageViewCount": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
