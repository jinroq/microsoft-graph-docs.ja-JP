---
title: Devicemanagementsettingstringlength 制約リソースの種類
description: 指定した文字列の長さの範囲を適用する制約
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5210808e511ac8f2a5d838c705bea583eb839f27
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364615"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="b2e9c-103">Devicemanagementsettingstringlength 制約リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2e9c-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

> <span data-ttu-id="b2e9c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2e9c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2e9c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b2e9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2e9c-106">指定した文字列の長さの範囲を適用する制約</span><span class="sxs-lookup"><span data-stu-id="b2e9c-106">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="b2e9c-107">[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b2e9c-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b2e9c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2e9c-108">Properties</span></span>
|<span data-ttu-id="b2e9c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2e9c-109">Property</span></span>|<span data-ttu-id="b2e9c-110">型</span><span class="sxs-lookup"><span data-stu-id="b2e9c-110">Type</span></span>|<span data-ttu-id="b2e9c-111">説明</span><span class="sxs-lookup"><span data-stu-id="b2e9c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2e9c-112">minimumLength</span><span class="sxs-lookup"><span data-stu-id="b2e9c-112">minimumLength</span></span>|<span data-ttu-id="b2e9c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b2e9c-113">Int32</span></span>|<span data-ttu-id="b2e9c-114">許可される最小文字列の長さ</span><span class="sxs-lookup"><span data-stu-id="b2e9c-114">The minimum permitted string length</span></span>|
|<span data-ttu-id="b2e9c-115">maximumLength</span><span class="sxs-lookup"><span data-stu-id="b2e9c-115">maximumLength</span></span>|<span data-ttu-id="b2e9c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b2e9c-116">Int32</span></span>|<span data-ttu-id="b2e9c-117">許可される最大文字列長</span><span class="sxs-lookup"><span data-stu-id="b2e9c-117">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2e9c-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b2e9c-118">Relationships</span></span>
<span data-ttu-id="b2e9c-119">なし</span><span class="sxs-lookup"><span data-stu-id="b2e9c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2e9c-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2e9c-120">JSON Representation</span></span>
<span data-ttu-id="b2e9c-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b2e9c-121">Here is a JSON representation of the resource.</span></span>
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



