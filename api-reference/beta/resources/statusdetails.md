---
title: statusDetails リソースの種類
description: プロビジョニングイベントとそれに関連するエラーの状態について説明します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d3c22e67af690a28bb974a0334af7891f0c25cfb
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349421"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="851c9-103">statusDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="851c9-103">statusDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="851c9-104">プロビジョニングイベントとそれに関連するエラーの状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="851c9-104">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="851c9-105">[Statusbase](/graph/api/resources/statusBase?view=graph-rest-beta)から継承され、状態が "失敗" に設定されている場合にのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="851c9-105">It is inherited from [statusBase](/graph/api/resources/statusBase?view=graph-rest-beta) and only used when status is set to 'failure'.</span></span>  

## <a name="properties"></a><span data-ttu-id="851c9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="851c9-106">Properties</span></span>

| <span data-ttu-id="851c9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="851c9-107">Property</span></span>     | <span data-ttu-id="851c9-108">型</span><span class="sxs-lookup"><span data-stu-id="851c9-108">Type</span></span>        | <span data-ttu-id="851c9-109">説明</span><span class="sxs-lookup"><span data-stu-id="851c9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="851c9-110">status</span><span class="sxs-lookup"><span data-stu-id="851c9-110">status</span></span>|<span data-ttu-id="851c9-111">String</span><span class="sxs-lookup"><span data-stu-id="851c9-111">String</span></span>|<span data-ttu-id="851c9-112">使用可能な値: `success`、`failure`、`skipped`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="851c9-112">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="851c9-113">StatusBase から継承されます。</span><span class="sxs-lookup"><span data-stu-id="851c9-113">Inherited from statusBase.</span></span>|
|<span data-ttu-id="851c9-114">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="851c9-114">additionalDetails</span></span>|<span data-ttu-id="851c9-115">String</span><span class="sxs-lookup"><span data-stu-id="851c9-115">String</span></span>|<span data-ttu-id="851c9-116">エラーが発生した場合の追加情報。</span><span class="sxs-lookup"><span data-stu-id="851c9-116">Additional details in case of error.</span></span>|
|<span data-ttu-id="851c9-117">errorCategory</span><span class="sxs-lookup"><span data-stu-id="851c9-117">errorCategory</span></span>|<span data-ttu-id="851c9-118">String</span><span class="sxs-lookup"><span data-stu-id="851c9-118">String</span></span>|<span data-ttu-id="851c9-119">エラーコードを分類します。</span><span class="sxs-lookup"><span data-stu-id="851c9-119">Categorizes the error code.</span></span>|
|<span data-ttu-id="851c9-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="851c9-120">errorCode</span></span>|<span data-ttu-id="851c9-121">String</span><span class="sxs-lookup"><span data-stu-id="851c9-121">String</span></span>|<span data-ttu-id="851c9-122">エラーが発生した場合は、一意のエラーコード。</span><span class="sxs-lookup"><span data-stu-id="851c9-122">Unique error code if any occurred.</span></span>|
|<span data-ttu-id="851c9-123">したがっ</span><span class="sxs-lookup"><span data-stu-id="851c9-123">reason</span></span>|<span data-ttu-id="851c9-124">String</span><span class="sxs-lookup"><span data-stu-id="851c9-124">String</span></span>|<span data-ttu-id="851c9-125">状態の概要と、状態が発生した理由を説明します。</span><span class="sxs-lookup"><span data-stu-id="851c9-125">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="851c9-126">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="851c9-126">recommendedAction</span></span>|<span data-ttu-id="851c9-127">String</span><span class="sxs-lookup"><span data-stu-id="851c9-127">String</span></span>|<span data-ttu-id="851c9-128">対応するエラーの解決方法を示します。</span><span class="sxs-lookup"><span data-stu-id="851c9-128">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="851c9-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="851c9-129">JSON representation</span></span>

<span data-ttu-id="851c9-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="851c9-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusDetails",
  "baseType": "microsoft.graph.statusBase"
}-->

```json
{
  "status": "failure",
  "additionalDetails": "String",
  "errorCategory": "String",
  "errorCode": "String",
  "reason": "String",
  "recommendedAction": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
