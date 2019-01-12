---
title: office365GroupsActivityFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: adff009d9047aa147c8042059fbdab8491288fb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972559"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="c3394-103">office365GroupsActivityFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c3394-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c3394-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3394-104">Properties</span></span>

| <span data-ttu-id="c3394-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3394-105">Property</span></span>          | <span data-ttu-id="c3394-106">種類</span><span class="sxs-lookup"><span data-stu-id="c3394-106">Type</span></span>   | <span data-ttu-id="c3394-107">説明</span><span class="sxs-lookup"><span data-stu-id="c3394-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="c3394-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c3394-108">reportRefreshDate</span></span> | <span data-ttu-id="c3394-109">日付</span><span class="sxs-lookup"><span data-stu-id="c3394-109">Date</span></span>   | <span data-ttu-id="c3394-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="c3394-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="c3394-111">total</span><span class="sxs-lookup"><span data-stu-id="c3394-111">total</span></span>             | <span data-ttu-id="c3394-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c3394-112">Int64</span></span>  | <span data-ttu-id="c3394-113">グループの SharePoint ドキュメント ライブラリ内のファイルの合計数です。</span><span class="sxs-lookup"><span data-stu-id="c3394-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="c3394-114">アクティブです</span><span class="sxs-lookup"><span data-stu-id="c3394-114">active</span></span>            | <span data-ttu-id="c3394-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c3394-115">Int64</span></span>  | <span data-ttu-id="c3394-116">、表示されたファイルの数は、編集、共有、またはグループの SharePoint ドキュメント ライブラリに同期します。</span><span class="sxs-lookup"><span data-stu-id="c3394-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="c3394-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="c3394-117">reportDate</span></span>        | <span data-ttu-id="c3394-118">日付</span><span class="sxs-lookup"><span data-stu-id="c3394-118">Date</span></span>   | <span data-ttu-id="c3394-119">グループの SharePoint サイトにアクティブだったファイルの数の日付です。</span><span class="sxs-lookup"><span data-stu-id="c3394-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="c3394-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c3394-120">reportPeriod</span></span>      | <span data-ttu-id="c3394-121">String</span><span class="sxs-lookup"><span data-stu-id="c3394-121">String</span></span> | <span data-ttu-id="c3394-122">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="c3394-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="c3394-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3394-123">JSON representation</span></span>

<span data-ttu-id="c3394-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c3394-124">The following is a JSON representation of the resource.</span></span>

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
