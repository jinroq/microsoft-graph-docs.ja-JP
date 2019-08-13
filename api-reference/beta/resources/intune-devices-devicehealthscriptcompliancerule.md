---
title: deviceHealthScriptComplianceRule リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8098582bd3e1b91a7e80af141e31847d2d3155cc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371539"
---
# <a name="devicehealthscriptcompliancerule-resource-type"></a><span data-ttu-id="4d9e8-103">deviceHealthScriptComplianceRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4d9e8-103">deviceHealthScriptComplianceRule resource type</span></span>

> <span data-ttu-id="4d9e8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d9e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d9e8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4d9e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d9e8-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4d9e8-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4d9e8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d9e8-107">Properties</span></span>
|<span data-ttu-id="4d9e8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d9e8-108">Property</span></span>|<span data-ttu-id="4d9e8-109">型</span><span class="sxs-lookup"><span data-stu-id="4d9e8-109">Type</span></span>|<span data-ttu-id="4d9e8-110">説明</span><span class="sxs-lookup"><span data-stu-id="4d9e8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d9e8-111">detectionType</span><span class="sxs-lookup"><span data-stu-id="4d9e8-111">detectionType</span></span>|[<span data-ttu-id="4d9e8-112">deviceHealthScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="4d9e8-112">deviceHealthScriptDetectionType</span></span>](../resources/intune-devices-devicehealthscriptdetectiontype.md)|<span data-ttu-id="4d9e8-113">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="4d9e8-113">Not yet documented.</span></span> <span data-ttu-id="4d9e8-114">可能な値は、`notConfigured`、`string` です。</span><span class="sxs-lookup"><span data-stu-id="4d9e8-114">Possible values are: `notConfigured`, `string`.</span></span>|
|<span data-ttu-id="4d9e8-115">operator</span><span class="sxs-lookup"><span data-stu-id="4d9e8-115">operator</span></span>|[<span data-ttu-id="4d9e8-116">deviceHealthScriptComplianceRuleOperator</span><span class="sxs-lookup"><span data-stu-id="4d9e8-116">deviceHealthScriptComplianceRuleOperator</span></span>](../resources/intune-devices-devicehealthscriptcomplianceruleoperator.md)|<span data-ttu-id="4d9e8-117">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="4d9e8-117">Not yet documented.</span></span> <span data-ttu-id="4d9e8-118">可能な値は、`notConfigured`、`equal`、`notEqual` です。</span><span class="sxs-lookup"><span data-stu-id="4d9e8-118">Possible values are: `notConfigured`, `equal`, `notEqual`.</span></span>|
|<span data-ttu-id="4d9e8-119">detectionValue</span><span class="sxs-lookup"><span data-stu-id="4d9e8-119">detectionValue</span></span>|<span data-ttu-id="4d9e8-120">String</span><span class="sxs-lookup"><span data-stu-id="4d9e8-120">String</span></span>|<span data-ttu-id="4d9e8-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4d9e8-121">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d9e8-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4d9e8-122">Relationships</span></span>
<span data-ttu-id="4d9e8-123">なし</span><span class="sxs-lookup"><span data-stu-id="4d9e8-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d9e8-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4d9e8-124">JSON Representation</span></span>
<span data-ttu-id="4d9e8-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4d9e8-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptComplianceRule",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```



