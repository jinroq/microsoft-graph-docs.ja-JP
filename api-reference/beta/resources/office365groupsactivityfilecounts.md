---
title: office365GroupsActivityFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: eb2d967108d4f75064b91670ae43fb7a2dd7ce7a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067668"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="ebc96-103">office365GroupsActivityFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ebc96-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ebc96-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebc96-104">Properties</span></span>

| <span data-ttu-id="ebc96-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebc96-105">Property</span></span>          | <span data-ttu-id="ebc96-106">型</span><span class="sxs-lookup"><span data-stu-id="ebc96-106">Type</span></span>   | <span data-ttu-id="ebc96-107">説明</span><span class="sxs-lookup"><span data-stu-id="ebc96-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="ebc96-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ebc96-108">reportRefreshDate</span></span> | <span data-ttu-id="ebc96-109">Date</span><span class="sxs-lookup"><span data-stu-id="ebc96-109">Date</span></span>   | <span data-ttu-id="ebc96-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="ebc96-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="ebc96-111">total</span><span class="sxs-lookup"><span data-stu-id="ebc96-111">total</span></span>             | <span data-ttu-id="ebc96-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ebc96-112">Int64</span></span>  | <span data-ttu-id="ebc96-113">グループの SharePoint ドキュメント ライブラリ内のファイルの合計数です。</span><span class="sxs-lookup"><span data-stu-id="ebc96-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="ebc96-114">アクティブです</span><span class="sxs-lookup"><span data-stu-id="ebc96-114">active</span></span>            | <span data-ttu-id="ebc96-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ebc96-115">Int64</span></span>  | <span data-ttu-id="ebc96-116">、表示されたファイルの数は、編集、共有、またはグループの SharePoint ドキュメント ライブラリに同期します。</span><span class="sxs-lookup"><span data-stu-id="ebc96-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="ebc96-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="ebc96-117">reportDate</span></span>        | <span data-ttu-id="ebc96-118">Date</span><span class="sxs-lookup"><span data-stu-id="ebc96-118">Date</span></span>   | <span data-ttu-id="ebc96-119">グループの SharePoint サイトにアクティブだったファイルの数の日付です。</span><span class="sxs-lookup"><span data-stu-id="ebc96-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="ebc96-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ebc96-120">reportPeriod</span></span>      | <span data-ttu-id="ebc96-121">String</span><span class="sxs-lookup"><span data-stu-id="ebc96-121">String</span></span> | <span data-ttu-id="ebc96-122">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="ebc96-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="ebc96-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ebc96-123">JSON representation</span></span>

<span data-ttu-id="ebc96-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ebc96-124">The following is a JSON representation of the resource.</span></span>

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
