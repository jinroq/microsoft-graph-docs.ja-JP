---
title: iosVppAppAssignmentSettings リソースの種類
description: グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bb4fd7e4a2cded97bdd5d61921cd1819908a4d77
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366778"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="aed14-103">iosVppAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aed14-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="aed14-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aed14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aed14-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aed14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aed14-106">グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="aed14-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="aed14-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="aed14-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aed14-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aed14-108">Properties</span></span>
|<span data-ttu-id="aed14-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aed14-109">Property</span></span>|<span data-ttu-id="aed14-110">型</span><span class="sxs-lookup"><span data-stu-id="aed14-110">Type</span></span>|<span data-ttu-id="aed14-111">説明</span><span class="sxs-lookup"><span data-stu-id="aed14-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aed14-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="aed14-112">useDeviceLicensing</span></span>|<span data-ttu-id="aed14-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="aed14-113">Boolean</span></span>|<span data-ttu-id="aed14-114">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="aed14-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="aed14-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="aed14-115">vpnConfigurationId</span></span>|<span data-ttu-id="aed14-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="aed14-116">String</span></span>|<span data-ttu-id="aed14-117">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="aed14-117">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="aed14-118">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="aed14-118">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="aed14-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="aed14-119">Boolean</span></span>|<span data-ttu-id="aed14-120">デバイスが Intune から削除されたときにアプリをアンインストールするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="aed14-120">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aed14-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aed14-121">Relationships</span></span>
<span data-ttu-id="aed14-122">なし</span><span class="sxs-lookup"><span data-stu-id="aed14-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aed14-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aed14-123">JSON Representation</span></span>
<span data-ttu-id="aed14-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aed14-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```



