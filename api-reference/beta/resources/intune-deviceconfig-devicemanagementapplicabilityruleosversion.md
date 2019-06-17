---
title: Devicemanagementの信頼性ルール Osversion リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c90a026a231998d7cd3ae25ab55ce63c5edb553
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002505"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="2a58e-103">Devicemanagementの信頼性ルール Osversion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2a58e-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

> <span data-ttu-id="2a58e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a58e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a58e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2a58e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a58e-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2a58e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2a58e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a58e-107">Properties</span></span>
|<span data-ttu-id="2a58e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a58e-108">Property</span></span>|<span data-ttu-id="2a58e-109">型</span><span class="sxs-lookup"><span data-stu-id="2a58e-109">Type</span></span>|<span data-ttu-id="2a58e-110">説明</span><span class="sxs-lookup"><span data-stu-id="2a58e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a58e-111">minOSVersion</span><span class="sxs-lookup"><span data-stu-id="2a58e-111">minOSVersion</span></span>|<span data-ttu-id="2a58e-112">String</span><span class="sxs-lookup"><span data-stu-id="2a58e-112">String</span></span>|<span data-ttu-id="2a58e-113">適用ルールの最小 OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="2a58e-113">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="2a58e-114">maxOSVersion</span><span class="sxs-lookup"><span data-stu-id="2a58e-114">maxOSVersion</span></span>|<span data-ttu-id="2a58e-115">String</span><span class="sxs-lookup"><span data-stu-id="2a58e-115">String</span></span>|<span data-ttu-id="2a58e-116">適用ルールの最大 OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="2a58e-116">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="2a58e-117">name</span><span class="sxs-lookup"><span data-stu-id="2a58e-117">name</span></span>|<span data-ttu-id="2a58e-118">String</span><span class="sxs-lookup"><span data-stu-id="2a58e-118">String</span></span>|<span data-ttu-id="2a58e-119">オブジェクトの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a58e-119">Name for object.</span></span>|
|<span data-ttu-id="2a58e-120">ruleType</span><span class="sxs-lookup"><span data-stu-id="2a58e-120">ruleType</span></span>|[<span data-ttu-id="2a58e-121">Devicemanagementの信頼性ルールの種類</span><span class="sxs-lookup"><span data-stu-id="2a58e-121">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="2a58e-122">適用性ルールの種類。</span><span class="sxs-lookup"><span data-stu-id="2a58e-122">Applicability Rule type.</span></span> <span data-ttu-id="2a58e-123">可能な値: `include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="2a58e-123">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a58e-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2a58e-124">Relationships</span></span>
<span data-ttu-id="2a58e-125">なし</span><span class="sxs-lookup"><span data-stu-id="2a58e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a58e-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2a58e-126">JSON Representation</span></span>
<span data-ttu-id="2a58e-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2a58e-127">Here is a JSON representation of the resource.</span></span>
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





