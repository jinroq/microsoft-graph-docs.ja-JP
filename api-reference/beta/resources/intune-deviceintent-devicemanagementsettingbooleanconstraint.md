---
title: deviceManagementSettingBooleanConstraint リソースの種類
description: 制約によって特定のブール値が適用されます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c39fbb19439572b1e698b3c5db3bcf0bf6c8ea5
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523694"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="92020-103">deviceManagementSettingBooleanConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92020-103">deviceManagementSettingBooleanConstraint resource type</span></span>

> <span data-ttu-id="92020-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92020-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92020-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92020-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92020-106">制約によって特定のブール値が適用されます。</span><span class="sxs-lookup"><span data-stu-id="92020-106">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="92020-107">[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="92020-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92020-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92020-108">Properties</span></span>
|<span data-ttu-id="92020-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92020-109">Property</span></span>|<span data-ttu-id="92020-110">型</span><span class="sxs-lookup"><span data-stu-id="92020-110">Type</span></span>|<span data-ttu-id="92020-111">説明</span><span class="sxs-lookup"><span data-stu-id="92020-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92020-112">value</span><span class="sxs-lookup"><span data-stu-id="92020-112">value</span></span>|<span data-ttu-id="92020-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="92020-113">Boolean</span></span>|<span data-ttu-id="92020-114">比較するブール値</span><span class="sxs-lookup"><span data-stu-id="92020-114">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="92020-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="92020-115">Relationships</span></span>
<span data-ttu-id="92020-116">なし</span><span class="sxs-lookup"><span data-stu-id="92020-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92020-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92020-117">JSON Representation</span></span>
<span data-ttu-id="92020-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="92020-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingBooleanConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingBooleanConstraint",
  "value": true
}
```







