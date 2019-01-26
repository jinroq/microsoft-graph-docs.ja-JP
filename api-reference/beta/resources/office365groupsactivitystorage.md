---
title: office365GroupsActivityStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576382"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="29ce3-103">office365GroupsActivityStorage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29ce3-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="29ce3-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29ce3-104">Properties</span></span>

| <span data-ttu-id="29ce3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29ce3-105">Property</span></span>                  | <span data-ttu-id="29ce3-106">型</span><span class="sxs-lookup"><span data-stu-id="29ce3-106">Type</span></span>   | <span data-ttu-id="29ce3-107">説明</span><span class="sxs-lookup"><span data-stu-id="29ce3-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="29ce3-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="29ce3-108">reportRefreshDate</span></span>         | <span data-ttu-id="29ce3-109">日付</span><span class="sxs-lookup"><span data-stu-id="29ce3-109">Date</span></span>   | <span data-ttu-id="29ce3-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="29ce3-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="29ce3-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="29ce3-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="29ce3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="29ce3-112">Int64</span></span>  | <span data-ttu-id="29ce3-113">ストレージ グループのメールボックスで使用されています。</span><span class="sxs-lookup"><span data-stu-id="29ce3-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="29ce3-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="29ce3-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="29ce3-115">Int64</span><span class="sxs-lookup"><span data-stu-id="29ce3-115">Int64</span></span>  | <span data-ttu-id="29ce3-116">SharePoint ドキュメント ライブラリで使用されている記憶域。</span><span class="sxs-lookup"><span data-stu-id="29ce3-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="29ce3-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="29ce3-117">reportDate</span></span>                | <span data-ttu-id="29ce3-118">日付</span><span class="sxs-lookup"><span data-stu-id="29ce3-118">Date</span></span>   | <span data-ttu-id="29ce3-119">Exchange と SharePoint のスナップショットの日付には、記憶域が使用されます。</span><span class="sxs-lookup"><span data-stu-id="29ce3-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="29ce3-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="29ce3-120">reportPeriod</span></span>              | <span data-ttu-id="29ce3-121">String</span><span class="sxs-lookup"><span data-stu-id="29ce3-121">String</span></span> | <span data-ttu-id="29ce3-122">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="29ce3-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="29ce3-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29ce3-123">JSON representation</span></span>

<span data-ttu-id="29ce3-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="29ce3-124">The following is a JSON representation of the resource.</span></span>

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
