---
title: Devicemanagementの信頼性ルール Osversion リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a81e8d096e8c11d6e1b3dd5117af1b384268095
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332849"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="dcde2-103">Devicemanagementの信頼性ルール Osversion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dcde2-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

> <span data-ttu-id="dcde2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcde2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcde2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dcde2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcde2-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dcde2-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="dcde2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcde2-107">Properties</span></span>
|<span data-ttu-id="dcde2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcde2-108">Property</span></span>|<span data-ttu-id="dcde2-109">型</span><span class="sxs-lookup"><span data-stu-id="dcde2-109">Type</span></span>|<span data-ttu-id="dcde2-110">説明</span><span class="sxs-lookup"><span data-stu-id="dcde2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcde2-111">minOSVersion</span><span class="sxs-lookup"><span data-stu-id="dcde2-111">minOSVersion</span></span>|<span data-ttu-id="dcde2-112">String</span><span class="sxs-lookup"><span data-stu-id="dcde2-112">String</span></span>|<span data-ttu-id="dcde2-113">適用ルールの最小 OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="dcde2-113">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="dcde2-114">maxOSVersion</span><span class="sxs-lookup"><span data-stu-id="dcde2-114">maxOSVersion</span></span>|<span data-ttu-id="dcde2-115">String</span><span class="sxs-lookup"><span data-stu-id="dcde2-115">String</span></span>|<span data-ttu-id="dcde2-116">適用ルールの最大 OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="dcde2-116">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="dcde2-117">name</span><span class="sxs-lookup"><span data-stu-id="dcde2-117">name</span></span>|<span data-ttu-id="dcde2-118">String</span><span class="sxs-lookup"><span data-stu-id="dcde2-118">String</span></span>|<span data-ttu-id="dcde2-119">オブジェクトの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="dcde2-119">Name for object.</span></span>|
|<span data-ttu-id="dcde2-120">ruleType</span><span class="sxs-lookup"><span data-stu-id="dcde2-120">ruleType</span></span>|[<span data-ttu-id="dcde2-121">Devicemanagementの信頼性ルールの種類</span><span class="sxs-lookup"><span data-stu-id="dcde2-121">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="dcde2-122">適用性ルールの種類。</span><span class="sxs-lookup"><span data-stu-id="dcde2-122">Applicability Rule type.</span></span> <span data-ttu-id="dcde2-123">可能な値: `include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="dcde2-123">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcde2-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dcde2-124">Relationships</span></span>
<span data-ttu-id="dcde2-125">なし</span><span class="sxs-lookup"><span data-stu-id="dcde2-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcde2-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dcde2-126">JSON Representation</span></span>
<span data-ttu-id="dcde2-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dcde2-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
  "minOSVersion": "String",
  "maxOSVersion": "String",
  "name": "String",
  "ruleType": "String"
}
```



