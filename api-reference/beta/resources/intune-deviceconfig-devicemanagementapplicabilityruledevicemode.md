---
title: Devicemanagementの信頼性ルール Devicemode リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8465f9276e573a44c2b7d80663d1de66bed83bef
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002526"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="53c86-103">Devicemanagementの信頼性ルール Devicemode リソースの種類</span><span class="sxs-lookup"><span data-stu-id="53c86-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

> <span data-ttu-id="53c86-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53c86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53c86-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="53c86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53c86-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="53c86-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="53c86-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53c86-107">Properties</span></span>
|<span data-ttu-id="53c86-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53c86-108">Property</span></span>|<span data-ttu-id="53c86-109">型</span><span class="sxs-lookup"><span data-stu-id="53c86-109">Type</span></span>|<span data-ttu-id="53c86-110">説明</span><span class="sxs-lookup"><span data-stu-id="53c86-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53c86-111">deviceMode</span><span class="sxs-lookup"><span data-stu-id="53c86-111">deviceMode</span></span>|[<span data-ttu-id="53c86-112">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="53c86-112">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="53c86-113">デバイスモードの適用規則。</span><span class="sxs-lookup"><span data-stu-id="53c86-113">Applicability rule for device mode.</span></span> <span data-ttu-id="53c86-114">可能な値は、`standardConfiguration`、`sModeConfiguration` です。</span><span class="sxs-lookup"><span data-stu-id="53c86-114">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="53c86-115">name</span><span class="sxs-lookup"><span data-stu-id="53c86-115">name</span></span>|<span data-ttu-id="53c86-116">String</span><span class="sxs-lookup"><span data-stu-id="53c86-116">String</span></span>|<span data-ttu-id="53c86-117">オブジェクトの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="53c86-117">Name for object.</span></span>|
|<span data-ttu-id="53c86-118">ruleType</span><span class="sxs-lookup"><span data-stu-id="53c86-118">ruleType</span></span>|[<span data-ttu-id="53c86-119">Devicemanagementの信頼性ルールの種類</span><span class="sxs-lookup"><span data-stu-id="53c86-119">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="53c86-120">適用性ルールの種類。</span><span class="sxs-lookup"><span data-stu-id="53c86-120">Applicability Rule type.</span></span> <span data-ttu-id="53c86-121">可能な値: `include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="53c86-121">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53c86-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="53c86-122">Relationships</span></span>
<span data-ttu-id="53c86-123">なし</span><span class="sxs-lookup"><span data-stu-id="53c86-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53c86-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="53c86-124">JSON Representation</span></span>
<span data-ttu-id="53c86-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="53c86-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
  "deviceMode": "String",
  "name": "String",
  "ruleType": "String"
}
```





