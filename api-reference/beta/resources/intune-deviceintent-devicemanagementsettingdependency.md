---
title: deviceManagementSettingDependency リソースの種類
description: 設定の依存関係情報
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39fa333a9ad008df9b1e71a6ae36f1be160ff9ce
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984521"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="953e3-103">deviceManagementSettingDependency リソースの種類</span><span class="sxs-lookup"><span data-stu-id="953e3-103">deviceManagementSettingDependency resource type</span></span>

> <span data-ttu-id="953e3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="953e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="953e3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="953e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="953e3-106">設定の依存関係情報</span><span class="sxs-lookup"><span data-stu-id="953e3-106">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="953e3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="953e3-107">Properties</span></span>
|<span data-ttu-id="953e3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="953e3-108">Property</span></span>|<span data-ttu-id="953e3-109">型</span><span class="sxs-lookup"><span data-stu-id="953e3-109">Type</span></span>|<span data-ttu-id="953e3-110">説明</span><span class="sxs-lookup"><span data-stu-id="953e3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="953e3-111">definitionId</span><span class="sxs-lookup"><span data-stu-id="953e3-111">definitionId</span></span>|<span data-ttu-id="953e3-112">String</span><span class="sxs-lookup"><span data-stu-id="953e3-112">String</span></span>|<span data-ttu-id="953e3-113">設定の設定定義 ID が依存している</span><span class="sxs-lookup"><span data-stu-id="953e3-113">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="953e3-114">式</span><span class="sxs-lookup"><span data-stu-id="953e3-114">constraints</span></span>|<span data-ttu-id="953e3-115">[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="953e3-115">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="953e3-116">依存関係設定値の制約のコレクション</span><span class="sxs-lookup"><span data-stu-id="953e3-116">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="953e3-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="953e3-117">Relationships</span></span>
<span data-ttu-id="953e3-118">なし</span><span class="sxs-lookup"><span data-stu-id="953e3-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="953e3-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="953e3-119">JSON Representation</span></span>
<span data-ttu-id="953e3-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="953e3-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDependency",
  "definitionId": "String",
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ]
}
```





