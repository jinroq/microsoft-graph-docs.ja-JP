---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0bf4748d8dc083fe03b55b5ee88062ebb429f639
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422860"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="9d6c8-103">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9d6c8-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="9d6c8-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9d6c8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9d6c8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d6c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d6c8-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9d6c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d6c8-107">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="9d6c8-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="9d6c8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d6c8-108">Properties</span></span>
|<span data-ttu-id="9d6c8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d6c8-109">Property</span></span>|<span data-ttu-id="9d6c8-110">型</span><span class="sxs-lookup"><span data-stu-id="9d6c8-110">Type</span></span>|<span data-ttu-id="9d6c8-111">説明</span><span class="sxs-lookup"><span data-stu-id="9d6c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d6c8-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="9d6c8-112">platformBlocked</span></span>|<span data-ttu-id="9d6c8-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="9d6c8-113">Boolean</span></span>|<span data-ttu-id="9d6c8-114">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="9d6c8-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="9d6c8-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="9d6c8-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="9d6c8-116">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="9d6c8-116">Boolean</span></span>|<span data-ttu-id="9d6c8-117">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="9d6c8-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="9d6c8-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9d6c8-118">osMinimumVersion</span></span>|<span data-ttu-id="9d6c8-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9d6c8-119">String</span></span>|<span data-ttu-id="9d6c8-120">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="9d6c8-120">Min OS version supported</span></span>|
|<span data-ttu-id="9d6c8-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9d6c8-121">osMaximumVersion</span></span>|<span data-ttu-id="9d6c8-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9d6c8-122">String</span></span>|<span data-ttu-id="9d6c8-123">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="9d6c8-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d6c8-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9d6c8-124">Relationships</span></span>
<span data-ttu-id="9d6c8-125">なし</span><span class="sxs-lookup"><span data-stu-id="9d6c8-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d6c8-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9d6c8-126">JSON Representation</span></span>
<span data-ttu-id="9d6c8-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9d6c8-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```




