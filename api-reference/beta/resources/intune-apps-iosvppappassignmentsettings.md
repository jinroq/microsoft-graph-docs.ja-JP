---
title: iosVppAppAssignmentSettings リソースの種類
description: グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1148336c5fa868cea90f223e66bf3868775647c6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423679"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="f2024-103">iosVppAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2024-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="f2024-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f2024-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f2024-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2024-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2024-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f2024-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2024-107">グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="f2024-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="f2024-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f2024-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f2024-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2024-109">Properties</span></span>
|<span data-ttu-id="f2024-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2024-110">Property</span></span>|<span data-ttu-id="f2024-111">型</span><span class="sxs-lookup"><span data-stu-id="f2024-111">Type</span></span>|<span data-ttu-id="f2024-112">説明</span><span class="sxs-lookup"><span data-stu-id="f2024-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2024-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="f2024-113">useDeviceLicensing</span></span>|<span data-ttu-id="f2024-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="f2024-114">Boolean</span></span>|<span data-ttu-id="f2024-115">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f2024-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="f2024-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f2024-116">vpnConfigurationId</span></span>|<span data-ttu-id="f2024-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f2024-117">String</span></span>|<span data-ttu-id="f2024-118">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="f2024-118">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2024-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f2024-119">Relationships</span></span>
<span data-ttu-id="f2024-120">なし</span><span class="sxs-lookup"><span data-stu-id="f2024-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2024-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2024-121">JSON Representation</span></span>
<span data-ttu-id="f2024-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f2024-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```




