---
title: office365GroupsActivityGroupCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 12dc0121c8f37c694265fce0d6cb5f58e56e0966
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069167"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="4b40f-103">office365GroupsActivityGroupCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b40f-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4b40f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b40f-104">Properties</span></span>

| <span data-ttu-id="4b40f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b40f-105">Property</span></span>          | <span data-ttu-id="4b40f-106">型</span><span class="sxs-lookup"><span data-stu-id="4b40f-106">Type</span></span>   | <span data-ttu-id="4b40f-107">説明</span><span class="sxs-lookup"><span data-stu-id="4b40f-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="4b40f-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4b40f-108">reportRefreshDate</span></span> | <span data-ttu-id="4b40f-109">Date</span><span class="sxs-lookup"><span data-stu-id="4b40f-109">Date</span></span>   | <span data-ttu-id="4b40f-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="4b40f-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="4b40f-111">total</span><span class="sxs-lookup"><span data-stu-id="4b40f-111">total</span></span>             | <span data-ttu-id="4b40f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4b40f-112">Int64</span></span>  | <span data-ttu-id="4b40f-113">グループの合計数です。</span><span class="sxs-lookup"><span data-stu-id="4b40f-113">The total number of groups.</span></span>              |
| <span data-ttu-id="4b40f-114">アクティブです</span><span class="sxs-lookup"><span data-stu-id="4b40f-114">active</span></span>            | <span data-ttu-id="4b40f-115">Int64</span><span class="sxs-lookup"><span data-stu-id="4b40f-115">Int64</span></span>  | <span data-ttu-id="4b40f-116">アクティブなグループの数。</span><span class="sxs-lookup"><span data-stu-id="4b40f-116">The number of active groups.</span></span> <span data-ttu-id="4b40f-117">グループは、次のいずれかが発生した場合は、アクティブと見なされます: グループのメールボックスに受信した電子メールです。ユーザーを表示、編集、共有、または SharePoint ドキュメント ライブラリ内のファイルの同期ユーザーが SharePoint ページを表示ユーザーは、投稿、読み取り、または、Yammer グループ内のメッセージを気に入られました。</span><span class="sxs-lookup"><span data-stu-id="4b40f-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="4b40f-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="4b40f-118">reportDate</span></span>        | <span data-ttu-id="4b40f-119">Date</span><span class="sxs-lookup"><span data-stu-id="4b40f-119">Date</span></span>   | <span data-ttu-id="4b40f-120">いくつかのグループにアクティブだった日付。</span><span class="sxs-lookup"><span data-stu-id="4b40f-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="4b40f-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4b40f-121">reportPeriod</span></span>      | <span data-ttu-id="4b40f-122">String</span><span class="sxs-lookup"><span data-stu-id="4b40f-122">String</span></span> | <span data-ttu-id="4b40f-123">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="4b40f-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="4b40f-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b40f-124">JSON representation</span></span>

<span data-ttu-id="4b40f-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4b40f-125">The following is a JSON representation of the resource.</span></span>

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
