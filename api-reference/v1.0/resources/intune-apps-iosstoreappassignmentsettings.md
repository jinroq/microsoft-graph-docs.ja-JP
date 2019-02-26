---
title: iosStoreAppAssignmentSettings リソースの種類
description: グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d58490e97aec48f664ab6882198e4c1da3511e8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250314"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="48224-103">iosStoreAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="48224-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="48224-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="48224-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48224-105">グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="48224-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="48224-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="48224-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="48224-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48224-107">Properties</span></span>
|<span data-ttu-id="48224-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48224-108">Property</span></span>|<span data-ttu-id="48224-109">型</span><span class="sxs-lookup"><span data-stu-id="48224-109">Type</span></span>|<span data-ttu-id="48224-110">説明</span><span class="sxs-lookup"><span data-stu-id="48224-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48224-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="48224-111">vpnConfigurationId</span></span>|<span data-ttu-id="48224-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="48224-112">String</span></span>|<span data-ttu-id="48224-113">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="48224-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48224-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="48224-114">Relationships</span></span>
<span data-ttu-id="48224-115">なし</span><span class="sxs-lookup"><span data-stu-id="48224-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48224-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48224-116">JSON Representation</span></span>
<span data-ttu-id="48224-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="48224-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



