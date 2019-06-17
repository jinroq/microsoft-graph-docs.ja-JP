---
title: deviceManagementApplicabilityRuleOsEdition リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b3baa84aa90af11f18d6c3dcf8ee1aeafecd240
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002519"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a><span data-ttu-id="bb7f8-103">deviceManagementApplicabilityRuleOsEdition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb7f8-103">deviceManagementApplicabilityRuleOsEdition resource type</span></span>

> <span data-ttu-id="bb7f8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb7f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb7f8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb7f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb7f8-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="bb7f8-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bb7f8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb7f8-107">Properties</span></span>
|<span data-ttu-id="bb7f8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb7f8-108">Property</span></span>|<span data-ttu-id="bb7f8-109">型</span><span class="sxs-lookup"><span data-stu-id="bb7f8-109">Type</span></span>|<span data-ttu-id="bb7f8-110">説明</span><span class="sxs-lookup"><span data-stu-id="bb7f8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb7f8-111">osEditionTypes</span><span class="sxs-lookup"><span data-stu-id="bb7f8-111">osEditionTypes</span></span>|<span data-ttu-id="bb7f8-112">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bb7f8-112">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md) collection</span></span>|<span data-ttu-id="bb7f8-113">適用規則の OS エディションの種類。</span><span class="sxs-lookup"><span data-stu-id="bb7f8-113">Applicability rule OS edition type.</span></span>|
|<span data-ttu-id="bb7f8-114">name</span><span class="sxs-lookup"><span data-stu-id="bb7f8-114">name</span></span>|<span data-ttu-id="bb7f8-115">String</span><span class="sxs-lookup"><span data-stu-id="bb7f8-115">String</span></span>|<span data-ttu-id="bb7f8-116">オブジェクトの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="bb7f8-116">Name for object.</span></span>|
|<span data-ttu-id="bb7f8-117">ruleType</span><span class="sxs-lookup"><span data-stu-id="bb7f8-117">ruleType</span></span>|[<span data-ttu-id="bb7f8-118">Devicemanagementの信頼性ルールの種類</span><span class="sxs-lookup"><span data-stu-id="bb7f8-118">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="bb7f8-119">適用性ルールの種類。</span><span class="sxs-lookup"><span data-stu-id="bb7f8-119">Applicability Rule type.</span></span> <span data-ttu-id="bb7f8-120">可能な値: `include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="bb7f8-120">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb7f8-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb7f8-121">Relationships</span></span>
<span data-ttu-id="bb7f8-122">なし</span><span class="sxs-lookup"><span data-stu-id="bb7f8-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb7f8-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb7f8-123">JSON Representation</span></span>
<span data-ttu-id="bb7f8-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb7f8-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
  "osEditionTypes": [
    "String"
  ],
  "name": "String",
  "ruleType": "String"
}
```





