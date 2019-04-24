---
title: office365GroupsActivityFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 89ac23b89730ec98515d6d0d3c06867e57b19ed1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457075"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="676ed-103">office365GroupsActivityFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="676ed-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="676ed-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="676ed-104">Properties</span></span>

| <span data-ttu-id="676ed-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="676ed-105">Property</span></span>          | <span data-ttu-id="676ed-106">型</span><span class="sxs-lookup"><span data-stu-id="676ed-106">Type</span></span>   | <span data-ttu-id="676ed-107">説明</span><span class="sxs-lookup"><span data-stu-id="676ed-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="676ed-108">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="676ed-108">reportRefreshDate</span></span> | <span data-ttu-id="676ed-109">日付</span><span class="sxs-lookup"><span data-stu-id="676ed-109">Date</span></span>   | <span data-ttu-id="676ed-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="676ed-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="676ed-111">total</span><span class="sxs-lookup"><span data-stu-id="676ed-111">total</span></span>             | <span data-ttu-id="676ed-112">Int64</span><span class="sxs-lookup"><span data-stu-id="676ed-112">Int64</span></span>  | <span data-ttu-id="676ed-113">グループの SharePoint ドキュメントライブラリ内のファイルの合計数。</span><span class="sxs-lookup"><span data-stu-id="676ed-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="676ed-114">active</span><span class="sxs-lookup"><span data-stu-id="676ed-114">active</span></span>            | <span data-ttu-id="676ed-115">Int64</span><span class="sxs-lookup"><span data-stu-id="676ed-115">Int64</span></span>  | <span data-ttu-id="676ed-116">グループの SharePoint ドキュメントライブラリで表示、編集、共有、または同期されたファイルの数。</span><span class="sxs-lookup"><span data-stu-id="676ed-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="676ed-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="676ed-117">reportDate</span></span>        | <span data-ttu-id="676ed-118">日付</span><span class="sxs-lookup"><span data-stu-id="676ed-118">Date</span></span>   | <span data-ttu-id="676ed-119">グループの SharePoint サイトで数個のファイルがアクティブになった日付。</span><span class="sxs-lookup"><span data-stu-id="676ed-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="676ed-120">reportperiod</span><span class="sxs-lookup"><span data-stu-id="676ed-120">reportPeriod</span></span>      | <span data-ttu-id="676ed-121">String</span><span class="sxs-lookup"><span data-stu-id="676ed-121">String</span></span> | <span data-ttu-id="676ed-122">レポートの対象となる日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="676ed-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="676ed-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="676ed-123">JSON representation</span></span>

<span data-ttu-id="676ed-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="676ed-124">The following is a JSON representation of the resource.</span></span>

<!-- {

  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
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
