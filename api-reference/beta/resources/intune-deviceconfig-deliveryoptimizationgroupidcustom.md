---
title: deliveryOptimizationGroupIdCustom リソースの種類
description: カスタムグループ id の種類
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec3b00920d0ead3df5fe694e110825615f449ef4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177974"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="2e0aa-103">deliveryOptimizationGroupIdCustom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2e0aa-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="2e0aa-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e0aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e0aa-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2e0aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e0aa-106">カスタムグループ id の種類</span><span class="sxs-lookup"><span data-stu-id="2e0aa-106">Custom group id type</span></span>


<span data-ttu-id="2e0aa-107">[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="2e0aa-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2e0aa-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e0aa-108">Properties</span></span>
|<span data-ttu-id="2e0aa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e0aa-109">Property</span></span>|<span data-ttu-id="2e0aa-110">型</span><span class="sxs-lookup"><span data-stu-id="2e0aa-110">Type</span></span>|<span data-ttu-id="2e0aa-111">説明</span><span class="sxs-lookup"><span data-stu-id="2e0aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e0aa-112">groupidcustom</span><span class="sxs-lookup"><span data-stu-id="2e0aa-112">groupIdCustom</span></span>|<span data-ttu-id="2e0aa-113">String</span><span class="sxs-lookup"><span data-stu-id="2e0aa-113">String</span></span>|<span data-ttu-id="2e0aa-114">デバイスが属する任意のグループ ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="2e0aa-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e0aa-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e0aa-115">Relationships</span></span>
<span data-ttu-id="2e0aa-116">なし</span><span class="sxs-lookup"><span data-stu-id="2e0aa-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e0aa-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e0aa-117">JSON Representation</span></span>
<span data-ttu-id="2e0aa-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2e0aa-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdCustom",
  "groupIdCustom": "String"
}
```




