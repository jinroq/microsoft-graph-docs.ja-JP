---
title: Devicemanagementsettingstringlength 制約リソースの種類
description: 指定した文字列の長さの範囲を適用する制約
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7cdcdeb138dce2c5b201527a079e3ee2de03737
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984465"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="d4d88-103">Devicemanagementsettingstringlength 制約リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d4d88-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

> <span data-ttu-id="d4d88-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4d88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4d88-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4d88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4d88-106">指定した文字列の長さの範囲を適用する制約</span><span class="sxs-lookup"><span data-stu-id="d4d88-106">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="d4d88-107">[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d4d88-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d4d88-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4d88-108">Properties</span></span>
|<span data-ttu-id="d4d88-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4d88-109">Property</span></span>|<span data-ttu-id="d4d88-110">型</span><span class="sxs-lookup"><span data-stu-id="d4d88-110">Type</span></span>|<span data-ttu-id="d4d88-111">説明</span><span class="sxs-lookup"><span data-stu-id="d4d88-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4d88-112">minimumLength</span><span class="sxs-lookup"><span data-stu-id="d4d88-112">minimumLength</span></span>|<span data-ttu-id="d4d88-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d4d88-113">Int32</span></span>|<span data-ttu-id="d4d88-114">許可される最小文字列の長さ</span><span class="sxs-lookup"><span data-stu-id="d4d88-114">The minimum permitted string length</span></span>|
|<span data-ttu-id="d4d88-115">maximumLength</span><span class="sxs-lookup"><span data-stu-id="d4d88-115">maximumLength</span></span>|<span data-ttu-id="d4d88-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d4d88-116">Int32</span></span>|<span data-ttu-id="d4d88-117">許可される最大文字列長</span><span class="sxs-lookup"><span data-stu-id="d4d88-117">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4d88-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d4d88-118">Relationships</span></span>
<span data-ttu-id="d4d88-119">なし</span><span class="sxs-lookup"><span data-stu-id="d4d88-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4d88-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d4d88-120">JSON Representation</span></span>
<span data-ttu-id="d4d88-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d4d88-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingStringLengthConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingStringLengthConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```





