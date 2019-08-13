---
title: deviceManagementSettingDependency リソースの種類
description: 設定の依存関係情報
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 100a6d441e161c353425f2d890e9468ebb32f3e8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364664"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="8fd0c-103">deviceManagementSettingDependency リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8fd0c-103">deviceManagementSettingDependency resource type</span></span>

> <span data-ttu-id="8fd0c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fd0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fd0c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8fd0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fd0c-106">設定の依存関係情報</span><span class="sxs-lookup"><span data-stu-id="8fd0c-106">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="8fd0c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fd0c-107">Properties</span></span>
|<span data-ttu-id="8fd0c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fd0c-108">Property</span></span>|<span data-ttu-id="8fd0c-109">型</span><span class="sxs-lookup"><span data-stu-id="8fd0c-109">Type</span></span>|<span data-ttu-id="8fd0c-110">説明</span><span class="sxs-lookup"><span data-stu-id="8fd0c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fd0c-111">definitionId</span><span class="sxs-lookup"><span data-stu-id="8fd0c-111">definitionId</span></span>|<span data-ttu-id="8fd0c-112">String</span><span class="sxs-lookup"><span data-stu-id="8fd0c-112">String</span></span>|<span data-ttu-id="8fd0c-113">設定の設定定義 ID が依存している</span><span class="sxs-lookup"><span data-stu-id="8fd0c-113">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="8fd0c-114">式</span><span class="sxs-lookup"><span data-stu-id="8fd0c-114">constraints</span></span>|<span data-ttu-id="8fd0c-115">[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8fd0c-115">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="8fd0c-116">依存関係設定値の制約のコレクション</span><span class="sxs-lookup"><span data-stu-id="8fd0c-116">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fd0c-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8fd0c-117">Relationships</span></span>
<span data-ttu-id="8fd0c-118">なし</span><span class="sxs-lookup"><span data-stu-id="8fd0c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fd0c-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8fd0c-119">JSON Representation</span></span>
<span data-ttu-id="8fd0c-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8fd0c-120">Here is a JSON representation of the resource.</span></span>
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



