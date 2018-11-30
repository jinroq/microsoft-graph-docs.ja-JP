---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
ms.openlocfilehash: 4319ab0f36e12ddd28ca9bb6c7bfd48043228504
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067518"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="f9357-102">incompleteData リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f9357-102">incompleteData resource type</span></span>

 > <span data-ttu-id="f9357-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f9357-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9357-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9357-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9357-105">**IncompleteData**ファセットは、不完全なデータとリソースが生成されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="f9357-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="f9357-106">内でプロパティがについての情報を提供するには、不完全なデータがある理由です。</span><span class="sxs-lookup"><span data-stu-id="f9357-106">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9357-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f9357-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="f9357-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9357-108">Properties</span></span>

| <span data-ttu-id="f9357-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9357-109">Property</span></span>                  | <span data-ttu-id="f9357-110">型</span><span class="sxs-lookup"><span data-stu-id="f9357-110">Type</span></span>           | <span data-ttu-id="f9357-111">説明</span><span class="sxs-lookup"><span data-stu-id="f9357-111">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="f9357-112">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="f9357-112">missingDataBeforeDateTime</span></span> | <span data-ttu-id="f9357-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9357-113">DateTimeOffset</span></span> | <span data-ttu-id="f9357-114">サービスには、指定された時間の前にソース データがありません。</span><span class="sxs-lookup"><span data-stu-id="f9357-114">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="f9357-115">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="f9357-115">wasThrottled</span></span>              | <span data-ttu-id="f9357-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="f9357-116">Boolean</span></span>        | <span data-ttu-id="f9357-117">データの一部は、過剰な活動のため録画されませんでした。</span><span class="sxs-lookup"><span data-stu-id="f9357-117">Some data was not recorded due to excessive activity.</span></span>

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData"
} -->
