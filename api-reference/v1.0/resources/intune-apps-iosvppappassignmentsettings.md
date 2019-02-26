---
title: iosVppAppAssignmentSettings リソースの種類
description: グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1ff346b9ae786fdc2158a5386625f808e04c181
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261118"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="db514-103">iosVppAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="db514-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="db514-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="db514-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db514-105">グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="db514-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="db514-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="db514-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="db514-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db514-107">Properties</span></span>
|<span data-ttu-id="db514-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db514-108">Property</span></span>|<span data-ttu-id="db514-109">型</span><span class="sxs-lookup"><span data-stu-id="db514-109">Type</span></span>|<span data-ttu-id="db514-110">説明</span><span class="sxs-lookup"><span data-stu-id="db514-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db514-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="db514-111">useDeviceLicensing</span></span>|<span data-ttu-id="db514-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="db514-112">Boolean</span></span>|<span data-ttu-id="db514-113">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="db514-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="db514-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="db514-114">vpnConfigurationId</span></span>|<span data-ttu-id="db514-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="db514-115">String</span></span>|<span data-ttu-id="db514-116">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="db514-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db514-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="db514-117">Relationships</span></span>
<span data-ttu-id="db514-118">なし</span><span class="sxs-lookup"><span data-stu-id="db514-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db514-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="db514-119">JSON Representation</span></span>
<span data-ttu-id="db514-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="db514-120">Here is a JSON representation of the resource.</span></span>
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



