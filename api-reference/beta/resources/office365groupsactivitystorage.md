---
title: office365GroupsActivityStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 9824d3d172a8578f8a25a049c2d0d3b407bbc47e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862252"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="34b38-103">office365GroupsActivityStorage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="34b38-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="34b38-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34b38-104">Properties</span></span>

| <span data-ttu-id="34b38-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34b38-105">Property</span></span>                  | <span data-ttu-id="34b38-106">種類</span><span class="sxs-lookup"><span data-stu-id="34b38-106">Type</span></span>   | <span data-ttu-id="34b38-107">説明</span><span class="sxs-lookup"><span data-stu-id="34b38-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="34b38-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="34b38-108">reportRefreshDate</span></span>         | <span data-ttu-id="34b38-109">日付</span><span class="sxs-lookup"><span data-stu-id="34b38-109">Date</span></span>   | <span data-ttu-id="34b38-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="34b38-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="34b38-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="34b38-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="34b38-112">Int64</span><span class="sxs-lookup"><span data-stu-id="34b38-112">Int64</span></span>  | <span data-ttu-id="34b38-113">ストレージ グループのメールボックスで使用されています。</span><span class="sxs-lookup"><span data-stu-id="34b38-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="34b38-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="34b38-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="34b38-115">Int64</span><span class="sxs-lookup"><span data-stu-id="34b38-115">Int64</span></span>  | <span data-ttu-id="34b38-116">SharePoint ドキュメント ライブラリで使用されている記憶域。</span><span class="sxs-lookup"><span data-stu-id="34b38-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="34b38-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="34b38-117">reportDate</span></span>                | <span data-ttu-id="34b38-118">日付</span><span class="sxs-lookup"><span data-stu-id="34b38-118">Date</span></span>   | <span data-ttu-id="34b38-119">Exchange と SharePoint のスナップショットの日付には、記憶域が使用されます。</span><span class="sxs-lookup"><span data-stu-id="34b38-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="34b38-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="34b38-120">reportPeriod</span></span>              | <span data-ttu-id="34b38-121">String</span><span class="sxs-lookup"><span data-stu-id="34b38-121">String</span></span> | <span data-ttu-id="34b38-122">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="34b38-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="34b38-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34b38-123">JSON representation</span></span>

<span data-ttu-id="34b38-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="34b38-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailboxStorageUsedInBytes": 1024, 
  "siteStorageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
