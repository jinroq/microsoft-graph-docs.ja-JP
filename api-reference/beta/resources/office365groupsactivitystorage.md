---
title: office365GroupsActivityStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 180e60a52b397f969aa10cee5bc27bba934ad1e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944454"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="75419-103">office365GroupsActivityStorage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75419-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="75419-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75419-104">Properties</span></span>

| <span data-ttu-id="75419-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75419-105">Property</span></span>                  | <span data-ttu-id="75419-106">種類</span><span class="sxs-lookup"><span data-stu-id="75419-106">Type</span></span>   | <span data-ttu-id="75419-107">説明</span><span class="sxs-lookup"><span data-stu-id="75419-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="75419-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="75419-108">reportRefreshDate</span></span>         | <span data-ttu-id="75419-109">日付</span><span class="sxs-lookup"><span data-stu-id="75419-109">Date</span></span>   | <span data-ttu-id="75419-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="75419-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="75419-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="75419-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="75419-112">Int64</span><span class="sxs-lookup"><span data-stu-id="75419-112">Int64</span></span>  | <span data-ttu-id="75419-113">ストレージ グループのメールボックスで使用されています。</span><span class="sxs-lookup"><span data-stu-id="75419-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="75419-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="75419-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="75419-115">Int64</span><span class="sxs-lookup"><span data-stu-id="75419-115">Int64</span></span>  | <span data-ttu-id="75419-116">SharePoint ドキュメント ライブラリで使用されている記憶域。</span><span class="sxs-lookup"><span data-stu-id="75419-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="75419-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="75419-117">reportDate</span></span>                | <span data-ttu-id="75419-118">日付</span><span class="sxs-lookup"><span data-stu-id="75419-118">Date</span></span>   | <span data-ttu-id="75419-119">Exchange と SharePoint のスナップショットの日付には、記憶域が使用されます。</span><span class="sxs-lookup"><span data-stu-id="75419-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="75419-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="75419-120">reportPeriod</span></span>              | <span data-ttu-id="75419-121">String</span><span class="sxs-lookup"><span data-stu-id="75419-121">String</span></span> | <span data-ttu-id="75419-122">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="75419-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="75419-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75419-123">JSON representation</span></span>

<span data-ttu-id="75419-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="75419-124">The following is a JSON representation of the resource.</span></span>

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
