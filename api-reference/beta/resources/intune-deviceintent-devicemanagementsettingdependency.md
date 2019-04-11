---
title: devicemanagementsettingdependency リソースの種類
description: 設定の依存関係情報
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b506ff636cf2a44b466d531f60924cd7eaa2c7b3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775549"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="7afcb-103">devicemanagementsettingdependency リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7afcb-103">deviceManagementSettingDependency resource type</span></span>

> <span data-ttu-id="7afcb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7afcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7afcb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7afcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7afcb-106">設定の依存関係情報</span><span class="sxs-lookup"><span data-stu-id="7afcb-106">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="7afcb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7afcb-107">Properties</span></span>
|<span data-ttu-id="7afcb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7afcb-108">Property</span></span>|<span data-ttu-id="7afcb-109">型</span><span class="sxs-lookup"><span data-stu-id="7afcb-109">Type</span></span>|<span data-ttu-id="7afcb-110">説明</span><span class="sxs-lookup"><span data-stu-id="7afcb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7afcb-111">definitionId</span><span class="sxs-lookup"><span data-stu-id="7afcb-111">definitionId</span></span>|<span data-ttu-id="7afcb-112">文字列</span><span class="sxs-lookup"><span data-stu-id="7afcb-112">String</span></span>|<span data-ttu-id="7afcb-113">設定の設定定義 ID が依存している</span><span class="sxs-lookup"><span data-stu-id="7afcb-113">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="7afcb-114">式</span><span class="sxs-lookup"><span data-stu-id="7afcb-114">constraints</span></span>|<span data-ttu-id="7afcb-115">[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7afcb-115">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="7afcb-116">依存関係設定値の制約のコレクション</span><span class="sxs-lookup"><span data-stu-id="7afcb-116">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="7afcb-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7afcb-117">Relationships</span></span>
<span data-ttu-id="7afcb-118">なし</span><span class="sxs-lookup"><span data-stu-id="7afcb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7afcb-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7afcb-119">JSON Representation</span></span>
<span data-ttu-id="7afcb-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7afcb-120">Here is a JSON representation of the resource.</span></span>
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





