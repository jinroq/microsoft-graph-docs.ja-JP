---
title: office365GroupsActivityStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: a3168ad417f246017ba1018aca265ec0363c951e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009462"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="ef719-103">office365GroupsActivityStorage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef719-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ef719-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef719-104">Properties</span></span>

| <span data-ttu-id="ef719-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef719-105">Property</span></span>                  | <span data-ttu-id="ef719-106">型</span><span class="sxs-lookup"><span data-stu-id="ef719-106">Type</span></span>   | <span data-ttu-id="ef719-107">説明</span><span class="sxs-lookup"><span data-stu-id="ef719-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="ef719-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ef719-108">reportRefreshDate</span></span>         | <span data-ttu-id="ef719-109">日付</span><span class="sxs-lookup"><span data-stu-id="ef719-109">Date</span></span>   | <span data-ttu-id="ef719-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="ef719-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="ef719-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="ef719-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="ef719-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ef719-112">Int64</span></span>  | <span data-ttu-id="ef719-113">グループメールボックスで使用されている記憶域。</span><span class="sxs-lookup"><span data-stu-id="ef719-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="ef719-114">Sitestorageused Inbytes</span><span class="sxs-lookup"><span data-stu-id="ef719-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="ef719-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ef719-115">Int64</span></span>  | <span data-ttu-id="ef719-116">SharePoint ドキュメントライブラリで使用されているストレージ。</span><span class="sxs-lookup"><span data-stu-id="ef719-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="ef719-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="ef719-117">reportDate</span></span>                | <span data-ttu-id="ef719-118">日付</span><span class="sxs-lookup"><span data-stu-id="ef719-118">Date</span></span>   | <span data-ttu-id="ef719-119">Exchange および SharePoint で使用されたストレージのスナップショット日付。</span><span class="sxs-lookup"><span data-stu-id="ef719-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="ef719-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ef719-120">reportPeriod</span></span>              | <span data-ttu-id="ef719-121">String</span><span class="sxs-lookup"><span data-stu-id="ef719-121">String</span></span> | <span data-ttu-id="ef719-122">レポートの対象となる日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="ef719-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="ef719-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef719-123">JSON representation</span></span>

<span data-ttu-id="ef719-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ef719-124">The following is a JSON representation of the resource.</span></span>

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
