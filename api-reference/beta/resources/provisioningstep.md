---
title: プロビジョニングステップリソースの種類
description: 'アクションを実行するために実行される手順について説明します。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1658114615c4532f0a7f9b9f5ad3c3a25deff81b
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349413"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="d0878-103">プロビジョニングステップリソースの種類</span><span class="sxs-lookup"><span data-stu-id="d0878-103">provisioningStep resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0878-104">アクションを実行するために実行される手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="d0878-104">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="d0878-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0878-105">Properties</span></span>

| <span data-ttu-id="d0878-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0878-106">Property</span></span>     | <span data-ttu-id="d0878-107">型</span><span class="sxs-lookup"><span data-stu-id="d0878-107">Type</span></span>        | <span data-ttu-id="d0878-108">説明</span><span class="sxs-lookup"><span data-stu-id="d0878-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d0878-109">description</span><span class="sxs-lookup"><span data-stu-id="d0878-109">description</span></span>|<span data-ttu-id="d0878-110">String</span><span class="sxs-lookup"><span data-stu-id="d0878-110">String</span></span>|<span data-ttu-id="d0878-111">手順中に発生した処理の概要。</span><span class="sxs-lookup"><span data-stu-id="d0878-111">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="d0878-112">詳細</span><span class="sxs-lookup"><span data-stu-id="d0878-112">details</span></span>|[<span data-ttu-id="d0878-113">詳細情報</span><span class="sxs-lookup"><span data-stu-id="d0878-113">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="d0878-114">手順中に発生した処理の詳細。</span><span class="sxs-lookup"><span data-stu-id="d0878-114">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="d0878-115">name</span><span class="sxs-lookup"><span data-stu-id="d0878-115">name</span></span>|<span data-ttu-id="d0878-116">文字列</span><span class="sxs-lookup"><span data-stu-id="d0878-116">String</span></span>|<span data-ttu-id="d0878-117">手順の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0878-117">Name of the step.</span></span>|
|<span data-ttu-id="d0878-118">/プロビジョニングの種類</span><span class="sxs-lookup"><span data-stu-id="d0878-118">provisioningStepType</span></span>|<span data-ttu-id="d0878-119">String</span><span class="sxs-lookup"><span data-stu-id="d0878-119">String</span></span>| <span data-ttu-id="d0878-120">手順の種類。</span><span class="sxs-lookup"><span data-stu-id="d0878-120">Type of step.</span></span> <span data-ttu-id="d0878-121">可能な値は、`import`、`scoping`、`matching`、`processing`、`referenceResolution`、`export`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="d0878-121">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d0878-122">status</span><span class="sxs-lookup"><span data-stu-id="d0878-122">status</span></span>|<span data-ttu-id="d0878-123">String</span><span class="sxs-lookup"><span data-stu-id="d0878-123">String</span></span>| <span data-ttu-id="d0878-124">手順の状態。</span><span class="sxs-lookup"><span data-stu-id="d0878-124">Status of the step.</span></span> <span data-ttu-id="d0878-125">使用可能な値は、`success`、`failure`、`skipped`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="d0878-125">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0878-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d0878-126">JSON representation</span></span>

<span data-ttu-id="d0878-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d0878-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStep",
  "baseType": null
}-->

```json
{
  "description": "String",
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "name": "String",
  "provisioningStepType": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStep resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
