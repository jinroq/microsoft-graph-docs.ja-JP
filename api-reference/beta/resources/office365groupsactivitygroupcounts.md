---
title: office365GroupsActivityGroupCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: ed5386083b11fb6fe7f063a4890744532feeb081
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832621"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="f7523-103">office365GroupsActivityGroupCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7523-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f7523-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7523-104">Properties</span></span>

| <span data-ttu-id="f7523-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7523-105">Property</span></span>          | <span data-ttu-id="f7523-106">種類</span><span class="sxs-lookup"><span data-stu-id="f7523-106">Type</span></span>   | <span data-ttu-id="f7523-107">説明</span><span class="sxs-lookup"><span data-stu-id="f7523-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="f7523-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f7523-108">reportRefreshDate</span></span> | <span data-ttu-id="f7523-109">日付</span><span class="sxs-lookup"><span data-stu-id="f7523-109">Date</span></span>   | <span data-ttu-id="f7523-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="f7523-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="f7523-111">total</span><span class="sxs-lookup"><span data-stu-id="f7523-111">total</span></span>             | <span data-ttu-id="f7523-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f7523-112">Int64</span></span>  | <span data-ttu-id="f7523-113">グループの合計数です。</span><span class="sxs-lookup"><span data-stu-id="f7523-113">The total number of groups.</span></span>              |
| <span data-ttu-id="f7523-114">アクティブです</span><span class="sxs-lookup"><span data-stu-id="f7523-114">active</span></span>            | <span data-ttu-id="f7523-115">Int64</span><span class="sxs-lookup"><span data-stu-id="f7523-115">Int64</span></span>  | <span data-ttu-id="f7523-116">アクティブなグループの数。</span><span class="sxs-lookup"><span data-stu-id="f7523-116">The number of active groups.</span></span> <span data-ttu-id="f7523-117">グループは、次のいずれかが発生した場合は、アクティブと見なされます: グループのメールボックスに受信した電子メールです。ユーザーを表示、編集、共有、または SharePoint ドキュメント ライブラリ内のファイルの同期ユーザーが SharePoint ページを表示ユーザーは、投稿、読み取り、または、Yammer グループ内のメッセージを気に入られました。</span><span class="sxs-lookup"><span data-stu-id="f7523-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="f7523-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="f7523-118">reportDate</span></span>        | <span data-ttu-id="f7523-119">日付</span><span class="sxs-lookup"><span data-stu-id="f7523-119">Date</span></span>   | <span data-ttu-id="f7523-120">いくつかのグループにアクティブだった日付。</span><span class="sxs-lookup"><span data-stu-id="f7523-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="f7523-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f7523-121">reportPeriod</span></span>      | <span data-ttu-id="f7523-122">String</span><span class="sxs-lookup"><span data-stu-id="f7523-122">String</span></span> | <span data-ttu-id="f7523-123">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="f7523-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="f7523-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7523-124">JSON representation</span></span>

<span data-ttu-id="f7523-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7523-125">The following is a JSON representation of the resource.</span></span>

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
