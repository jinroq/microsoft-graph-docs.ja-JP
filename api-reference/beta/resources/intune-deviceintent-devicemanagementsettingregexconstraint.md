---
title: deviceManagementSettingRegexConstraint リソースの種類
description: 指定された RegEx パターンに対して設定の一致を強制する制約
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bb05c0f58d3c30b18bd240c8047d34a3977e85b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943308"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="1c177-103">deviceManagementSettingRegexConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1c177-103">deviceManagementSettingRegexConstraint resource type</span></span>

> <span data-ttu-id="1c177-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c177-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c177-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1c177-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c177-106">指定された RegEx パターンに対して設定の一致を強制する制約</span><span class="sxs-lookup"><span data-stu-id="1c177-106">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="1c177-107">[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="1c177-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1c177-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c177-108">Properties</span></span>
|<span data-ttu-id="1c177-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c177-109">Property</span></span>|<span data-ttu-id="1c177-110">型</span><span class="sxs-lookup"><span data-stu-id="1c177-110">Type</span></span>|<span data-ttu-id="1c177-111">説明</span><span class="sxs-lookup"><span data-stu-id="1c177-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c177-112">pcre</span><span class="sxs-lookup"><span data-stu-id="1c177-112">regex</span></span>|<span data-ttu-id="1c177-113">String</span><span class="sxs-lookup"><span data-stu-id="1c177-113">String</span></span>|<span data-ttu-id="1c177-114">照合する正規表現パターン</span><span class="sxs-lookup"><span data-stu-id="1c177-114">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c177-115">関係</span><span class="sxs-lookup"><span data-stu-id="1c177-115">Relationships</span></span>
<span data-ttu-id="1c177-116">なし</span><span class="sxs-lookup"><span data-stu-id="1c177-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c177-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1c177-117">JSON Representation</span></span>
<span data-ttu-id="1c177-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1c177-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRegexConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRegexConstraint",
  "regex": "String"
}
```




