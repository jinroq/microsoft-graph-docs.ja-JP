---
title: deliveryOptimizationGroupIdCustom リソースの種類
description: カスタムグループ id の種類
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d4f369c9a3b62480549f19d4a7c1d7b1d0bb196
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796592"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="911cf-103">deliveryOptimizationGroupIdCustom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="911cf-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="911cf-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="911cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="911cf-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="911cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="911cf-106">カスタムグループ id の種類</span><span class="sxs-lookup"><span data-stu-id="911cf-106">Custom group id type</span></span>


<span data-ttu-id="911cf-107">[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="911cf-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="911cf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="911cf-108">Properties</span></span>
|<span data-ttu-id="911cf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="911cf-109">Property</span></span>|<span data-ttu-id="911cf-110">型</span><span class="sxs-lookup"><span data-stu-id="911cf-110">Type</span></span>|<span data-ttu-id="911cf-111">説明</span><span class="sxs-lookup"><span data-stu-id="911cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="911cf-112">groupidcustom</span><span class="sxs-lookup"><span data-stu-id="911cf-112">groupIdCustom</span></span>|<span data-ttu-id="911cf-113">文字列</span><span class="sxs-lookup"><span data-stu-id="911cf-113">String</span></span>|<span data-ttu-id="911cf-114">デバイスが属する任意のグループ ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="911cf-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="911cf-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="911cf-115">Relationships</span></span>
<span data-ttu-id="911cf-116">なし</span><span class="sxs-lookup"><span data-stu-id="911cf-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="911cf-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="911cf-117">JSON Representation</span></span>
<span data-ttu-id="911cf-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="911cf-118">Here is a JSON representation of the resource.</span></span>
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





