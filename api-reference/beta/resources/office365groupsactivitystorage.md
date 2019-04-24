---
title: office365GroupsActivityStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505551"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="06130-103">office365GroupsActivityStorage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06130-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="06130-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06130-104">Properties</span></span>

| <span data-ttu-id="06130-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06130-105">Property</span></span>                  | <span data-ttu-id="06130-106">型</span><span class="sxs-lookup"><span data-stu-id="06130-106">Type</span></span>   | <span data-ttu-id="06130-107">説明</span><span class="sxs-lookup"><span data-stu-id="06130-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="06130-108">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="06130-108">reportRefreshDate</span></span>         | <span data-ttu-id="06130-109">Date</span><span class="sxs-lookup"><span data-stu-id="06130-109">Date</span></span>   | <span data-ttu-id="06130-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="06130-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="06130-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="06130-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="06130-112">Int64</span><span class="sxs-lookup"><span data-stu-id="06130-112">Int64</span></span>  | <span data-ttu-id="06130-113">グループメールボックスで使用されている記憶域。</span><span class="sxs-lookup"><span data-stu-id="06130-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="06130-114">sitestorageused inbytes</span><span class="sxs-lookup"><span data-stu-id="06130-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="06130-115">Int64</span><span class="sxs-lookup"><span data-stu-id="06130-115">Int64</span></span>  | <span data-ttu-id="06130-116">SharePoint ドキュメントライブラリで使用されているストレージ。</span><span class="sxs-lookup"><span data-stu-id="06130-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="06130-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="06130-117">reportDate</span></span>                | <span data-ttu-id="06130-118">Date</span><span class="sxs-lookup"><span data-stu-id="06130-118">Date</span></span>   | <span data-ttu-id="06130-119">Exchange および SharePoint で使用されたストレージのスナップショット日付。</span><span class="sxs-lookup"><span data-stu-id="06130-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="06130-120">reportperiod</span><span class="sxs-lookup"><span data-stu-id="06130-120">reportPeriod</span></span>              | <span data-ttu-id="06130-121">String</span><span class="sxs-lookup"><span data-stu-id="06130-121">String</span></span> | <span data-ttu-id="06130-122">レポートの対象となる日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="06130-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="06130-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06130-123">JSON representation</span></span>

<span data-ttu-id="06130-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06130-124">The following is a JSON representation of the resource.</span></span>

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
