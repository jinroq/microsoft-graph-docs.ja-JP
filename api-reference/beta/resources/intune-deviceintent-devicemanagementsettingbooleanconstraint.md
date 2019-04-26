---
title: deviceManagementSettingBooleanConstraint リソースの種類
description: 制約によって特定のブール値が適用されます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee2689bfbc6b407a688c0422c568d4b311694c06
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562287"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="bb2cb-103">deviceManagementSettingBooleanConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb2cb-103">deviceManagementSettingBooleanConstraint resource type</span></span>

> <span data-ttu-id="bb2cb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb2cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb2cb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb2cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb2cb-106">制約によって特定のブール値が適用されます。</span><span class="sxs-lookup"><span data-stu-id="bb2cb-106">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="bb2cb-107">[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="bb2cb-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bb2cb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb2cb-108">Properties</span></span>
|<span data-ttu-id="bb2cb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb2cb-109">Property</span></span>|<span data-ttu-id="bb2cb-110">型</span><span class="sxs-lookup"><span data-stu-id="bb2cb-110">Type</span></span>|<span data-ttu-id="bb2cb-111">説明</span><span class="sxs-lookup"><span data-stu-id="bb2cb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb2cb-112">value</span><span class="sxs-lookup"><span data-stu-id="bb2cb-112">value</span></span>|<span data-ttu-id="bb2cb-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="bb2cb-113">Boolean</span></span>|<span data-ttu-id="bb2cb-114">比較するブール値</span><span class="sxs-lookup"><span data-stu-id="bb2cb-114">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb2cb-115">関係</span><span class="sxs-lookup"><span data-stu-id="bb2cb-115">Relationships</span></span>
<span data-ttu-id="bb2cb-116">なし</span><span class="sxs-lookup"><span data-stu-id="bb2cb-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb2cb-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb2cb-117">JSON Representation</span></span>
<span data-ttu-id="bb2cb-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb2cb-118">Here is a JSON representation of the resource.</span></span>
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





