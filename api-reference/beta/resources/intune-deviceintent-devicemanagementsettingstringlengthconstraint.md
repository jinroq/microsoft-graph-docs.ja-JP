---
title: devicemanagementsettingstringlength 制約リソースの種類
description: 指定した文字列の長さの範囲を適用する制約
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49d009571cdccf60dc8adcc2f1a703d39d0674c7
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522336"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="a394d-103">devicemanagementsettingstringlength 制約リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a394d-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

> <span data-ttu-id="a394d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a394d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a394d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a394d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a394d-106">指定した文字列の長さの範囲を適用する制約</span><span class="sxs-lookup"><span data-stu-id="a394d-106">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="a394d-107">[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="a394d-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a394d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a394d-108">Properties</span></span>
|<span data-ttu-id="a394d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a394d-109">Property</span></span>|<span data-ttu-id="a394d-110">型</span><span class="sxs-lookup"><span data-stu-id="a394d-110">Type</span></span>|<span data-ttu-id="a394d-111">説明</span><span class="sxs-lookup"><span data-stu-id="a394d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a394d-112">minimumlength</span><span class="sxs-lookup"><span data-stu-id="a394d-112">minimumLength</span></span>|<span data-ttu-id="a394d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a394d-113">Int32</span></span>|<span data-ttu-id="a394d-114">許可される最小文字列の長さ</span><span class="sxs-lookup"><span data-stu-id="a394d-114">The minimum permitted string length</span></span>|
|<span data-ttu-id="a394d-115">maximumlength</span><span class="sxs-lookup"><span data-stu-id="a394d-115">maximumLength</span></span>|<span data-ttu-id="a394d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a394d-116">Int32</span></span>|<span data-ttu-id="a394d-117">許可される最大文字列長</span><span class="sxs-lookup"><span data-stu-id="a394d-117">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="a394d-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a394d-118">Relationships</span></span>
<span data-ttu-id="a394d-119">なし</span><span class="sxs-lookup"><span data-stu-id="a394d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a394d-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a394d-120">JSON Representation</span></span>
<span data-ttu-id="a394d-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a394d-121">Here is a JSON representation of the resource.</span></span>
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







