---
title: deliveryOptimizationGroupIdCustom リソースの種類
description: カスタムグループ id の種類
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3dbddceca6f6b7adc023431a8b8157ce02ef379
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979649"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="aecf1-103">deliveryOptimizationGroupIdCustom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aecf1-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="aecf1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aecf1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aecf1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aecf1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aecf1-106">カスタムグループ id の種類</span><span class="sxs-lookup"><span data-stu-id="aecf1-106">Custom group id type</span></span>


<span data-ttu-id="aecf1-107">[DeliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="aecf1-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aecf1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aecf1-108">Properties</span></span>
|<span data-ttu-id="aecf1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aecf1-109">Property</span></span>|<span data-ttu-id="aecf1-110">型</span><span class="sxs-lookup"><span data-stu-id="aecf1-110">Type</span></span>|<span data-ttu-id="aecf1-111">説明</span><span class="sxs-lookup"><span data-stu-id="aecf1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aecf1-112">groupIdCustom</span><span class="sxs-lookup"><span data-stu-id="aecf1-112">groupIdCustom</span></span>|<span data-ttu-id="aecf1-113">String</span><span class="sxs-lookup"><span data-stu-id="aecf1-113">String</span></span>|<span data-ttu-id="aecf1-114">デバイスが属する任意のグループ ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="aecf1-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="aecf1-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aecf1-115">Relationships</span></span>
<span data-ttu-id="aecf1-116">なし</span><span class="sxs-lookup"><span data-stu-id="aecf1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aecf1-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aecf1-117">JSON Representation</span></span>
<span data-ttu-id="aecf1-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aecf1-118">Here is a JSON representation of the resource.</span></span>
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





