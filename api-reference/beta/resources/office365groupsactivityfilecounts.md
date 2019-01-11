---
title: office365GroupsActivityFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 856bb4c74c8af35775b6fe71cb75d89935440bdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819187"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="80b12-103">office365GroupsActivityFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="80b12-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="80b12-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80b12-104">Properties</span></span>

| <span data-ttu-id="80b12-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80b12-105">Property</span></span>          | <span data-ttu-id="80b12-106">種類</span><span class="sxs-lookup"><span data-stu-id="80b12-106">Type</span></span>   | <span data-ttu-id="80b12-107">説明</span><span class="sxs-lookup"><span data-stu-id="80b12-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="80b12-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="80b12-108">reportRefreshDate</span></span> | <span data-ttu-id="80b12-109">日付</span><span class="sxs-lookup"><span data-stu-id="80b12-109">Date</span></span>   | <span data-ttu-id="80b12-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="80b12-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="80b12-111">total</span><span class="sxs-lookup"><span data-stu-id="80b12-111">total</span></span>             | <span data-ttu-id="80b12-112">Int64</span><span class="sxs-lookup"><span data-stu-id="80b12-112">Int64</span></span>  | <span data-ttu-id="80b12-113">グループの SharePoint ドキュメント ライブラリ内のファイルの合計数です。</span><span class="sxs-lookup"><span data-stu-id="80b12-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="80b12-114">アクティブです</span><span class="sxs-lookup"><span data-stu-id="80b12-114">active</span></span>            | <span data-ttu-id="80b12-115">Int64</span><span class="sxs-lookup"><span data-stu-id="80b12-115">Int64</span></span>  | <span data-ttu-id="80b12-116">、表示されたファイルの数は、編集、共有、またはグループの SharePoint ドキュメント ライブラリに同期します。</span><span class="sxs-lookup"><span data-stu-id="80b12-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="80b12-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="80b12-117">reportDate</span></span>        | <span data-ttu-id="80b12-118">日付</span><span class="sxs-lookup"><span data-stu-id="80b12-118">Date</span></span>   | <span data-ttu-id="80b12-119">グループの SharePoint サイトにアクティブだったファイルの数の日付です。</span><span class="sxs-lookup"><span data-stu-id="80b12-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="80b12-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="80b12-120">reportPeriod</span></span>      | <span data-ttu-id="80b12-121">String</span><span class="sxs-lookup"><span data-stu-id="80b12-121">String</span></span> | <span data-ttu-id="80b12-122">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="80b12-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="80b12-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="80b12-123">JSON representation</span></span>

<span data-ttu-id="80b12-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="80b12-124">The following is a JSON representation of the resource.</span></span>

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
