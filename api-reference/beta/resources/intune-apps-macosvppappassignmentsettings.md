---
title: macOsVppAppAssignmentSettings リソースの種類
description: Mac VPP のモバイル アプリケーションをグループに割り当てるために使用するプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0927277b11416da001ad826200bf4ec841341118
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431672"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="6d9ba-103">macOsVppAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6d9ba-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="6d9ba-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6d9ba-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6d9ba-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d9ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d9ba-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6d9ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d9ba-107">Mac VPP のモバイル アプリケーションをグループに割り当てるために使用するプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6d9ba-107">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="6d9ba-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6d9ba-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6d9ba-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d9ba-109">Properties</span></span>
|<span data-ttu-id="6d9ba-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d9ba-110">Property</span></span>|<span data-ttu-id="6d9ba-111">型</span><span class="sxs-lookup"><span data-stu-id="6d9ba-111">Type</span></span>|<span data-ttu-id="6d9ba-112">説明</span><span class="sxs-lookup"><span data-stu-id="6d9ba-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d9ba-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="6d9ba-113">useDeviceLicensing</span></span>|<span data-ttu-id="6d9ba-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="6d9ba-114">Boolean</span></span>|<span data-ttu-id="6d9ba-115">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="6d9ba-115">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d9ba-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6d9ba-116">Relationships</span></span>
<span data-ttu-id="6d9ba-117">なし</span><span class="sxs-lookup"><span data-stu-id="6d9ba-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d9ba-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6d9ba-118">JSON Representation</span></span>
<span data-ttu-id="6d9ba-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6d9ba-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignmentSettings",
  "useDeviceLicensing": true
}
```




