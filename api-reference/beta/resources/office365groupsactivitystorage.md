---
title: office365GroupsActivityStorage リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 23ff4d112373f52c4c19d6631ac89bac22399b29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073258"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="7175d-103">office365GroupsActivityStorage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7175d-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7175d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7175d-104">Properties</span></span>

| <span data-ttu-id="7175d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7175d-105">Property</span></span>                  | <span data-ttu-id="7175d-106">型</span><span class="sxs-lookup"><span data-stu-id="7175d-106">Type</span></span>   | <span data-ttu-id="7175d-107">説明</span><span class="sxs-lookup"><span data-stu-id="7175d-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="7175d-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7175d-108">reportRefreshDate</span></span>         | <span data-ttu-id="7175d-109">Date</span><span class="sxs-lookup"><span data-stu-id="7175d-109">Date</span></span>   | <span data-ttu-id="7175d-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="7175d-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="7175d-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="7175d-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="7175d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7175d-112">Int64</span></span>  | <span data-ttu-id="7175d-113">ストレージ グループのメールボックスで使用されています。</span><span class="sxs-lookup"><span data-stu-id="7175d-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="7175d-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="7175d-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="7175d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="7175d-115">Int64</span></span>  | <span data-ttu-id="7175d-116">SharePoint ドキュメント ライブラリで使用されている記憶域。</span><span class="sxs-lookup"><span data-stu-id="7175d-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="7175d-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="7175d-117">reportDate</span></span>                | <span data-ttu-id="7175d-118">Date</span><span class="sxs-lookup"><span data-stu-id="7175d-118">Date</span></span>   | <span data-ttu-id="7175d-119">Exchange と SharePoint のスナップショットの日付には、記憶域が使用されます。</span><span class="sxs-lookup"><span data-stu-id="7175d-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="7175d-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7175d-120">reportPeriod</span></span>              | <span data-ttu-id="7175d-121">String</span><span class="sxs-lookup"><span data-stu-id="7175d-121">String</span></span> | <span data-ttu-id="7175d-122">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="7175d-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="7175d-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7175d-123">JSON representation</span></span>

<span data-ttu-id="7175d-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7175d-124">The following is a JSON representation of the resource.</span></span>

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
