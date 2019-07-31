---
title: office365GroupsActivityGroupCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 3f49ddaf6f62367c5e8ebbffae669bf3cc1d86f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009483"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="36332-103">office365GroupsActivityGroupCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="36332-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="36332-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36332-104">Properties</span></span>

| <span data-ttu-id="36332-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36332-105">Property</span></span>          | <span data-ttu-id="36332-106">型</span><span class="sxs-lookup"><span data-stu-id="36332-106">Type</span></span>   | <span data-ttu-id="36332-107">説明</span><span class="sxs-lookup"><span data-stu-id="36332-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="36332-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="36332-108">reportRefreshDate</span></span> | <span data-ttu-id="36332-109">日付</span><span class="sxs-lookup"><span data-stu-id="36332-109">Date</span></span>   | <span data-ttu-id="36332-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="36332-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="36332-111">total</span><span class="sxs-lookup"><span data-stu-id="36332-111">total</span></span>             | <span data-ttu-id="36332-112">Int64</span><span class="sxs-lookup"><span data-stu-id="36332-112">Int64</span></span>  | <span data-ttu-id="36332-113">グループの合計数。</span><span class="sxs-lookup"><span data-stu-id="36332-113">The total number of groups.</span></span>              |
| <span data-ttu-id="36332-114">active</span><span class="sxs-lookup"><span data-stu-id="36332-114">active</span></span>            | <span data-ttu-id="36332-115">Int64</span><span class="sxs-lookup"><span data-stu-id="36332-115">Int64</span></span>  | <span data-ttu-id="36332-116">アクティブなグループの数。</span><span class="sxs-lookup"><span data-stu-id="36332-116">The number of active groups.</span></span> <span data-ttu-id="36332-117">グループは、次のいずれかが発生した場合にアクティブと見なされます。グループメールが受信した電子メール。SharePoint ドキュメントライブラリでユーザーが表示、編集、共有、または同期されたファイル。ユーザーが SharePoint ページを表示した。Yammer グループ内のユーザー投稿、閲覧、またはいいねのメッセージ。</span><span class="sxs-lookup"><span data-stu-id="36332-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="36332-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="36332-118">reportDate</span></span>        | <span data-ttu-id="36332-119">日付</span><span class="sxs-lookup"><span data-stu-id="36332-119">Date</span></span>   | <span data-ttu-id="36332-120">グループの数がアクティブであった日付。</span><span class="sxs-lookup"><span data-stu-id="36332-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="36332-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="36332-121">reportPeriod</span></span>      | <span data-ttu-id="36332-122">String</span><span class="sxs-lookup"><span data-stu-id="36332-122">String</span></span> | <span data-ttu-id="36332-123">レポートの対象となる日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="36332-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="36332-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="36332-124">JSON representation</span></span>

<span data-ttu-id="36332-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="36332-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
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
