---
title: iosVppAppAssignmentSettings リソースの種類
description: グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d35cd60b1e616f38b8c4c792f7bd766f550b62aa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029121"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="6deab-103">iosVppAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6deab-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="6deab-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6deab-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6deab-105">グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="6deab-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="6deab-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6deab-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6deab-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6deab-107">Properties</span></span>
|<span data-ttu-id="6deab-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6deab-108">Property</span></span>|<span data-ttu-id="6deab-109">型</span><span class="sxs-lookup"><span data-stu-id="6deab-109">Type</span></span>|<span data-ttu-id="6deab-110">説明</span><span class="sxs-lookup"><span data-stu-id="6deab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6deab-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="6deab-111">useDeviceLicensing</span></span>|<span data-ttu-id="6deab-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="6deab-112">Boolean</span></span>|<span data-ttu-id="6deab-113">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="6deab-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="6deab-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="6deab-114">vpnConfigurationId</span></span>|<span data-ttu-id="6deab-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="6deab-115">String</span></span>|<span data-ttu-id="6deab-116">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="6deab-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6deab-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6deab-117">Relationships</span></span>
<span data-ttu-id="6deab-118">なし</span><span class="sxs-lookup"><span data-stu-id="6deab-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6deab-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6deab-119">JSON Representation</span></span>
<span data-ttu-id="6deab-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6deab-120">Here is a JSON representation of the resource.</span></span>
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



