---
title: iosVppAppAssignmentSettings リソースの種類
description: グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4c9a5196be760204af682c1a7318318920284a40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886115"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="4bea2-103">iosVppAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4bea2-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="4bea2-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4bea2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4bea2-105">グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="4bea2-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="4bea2-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4bea2-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4bea2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bea2-107">Properties</span></span>
|<span data-ttu-id="4bea2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bea2-108">Property</span></span>|<span data-ttu-id="4bea2-109">種類</span><span class="sxs-lookup"><span data-stu-id="4bea2-109">Type</span></span>|<span data-ttu-id="4bea2-110">説明</span><span class="sxs-lookup"><span data-stu-id="4bea2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bea2-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="4bea2-111">useDeviceLicensing</span></span>|<span data-ttu-id="4bea2-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="4bea2-112">Boolean</span></span>|<span data-ttu-id="4bea2-113">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="4bea2-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="4bea2-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="4bea2-114">vpnConfigurationId</span></span>|<span data-ttu-id="4bea2-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4bea2-115">String</span></span>|<span data-ttu-id="4bea2-116">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="4bea2-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bea2-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4bea2-117">Relationships</span></span>
<span data-ttu-id="4bea2-118">なし</span><span class="sxs-lookup"><span data-stu-id="4bea2-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4bea2-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4bea2-119">JSON Representation</span></span>
<span data-ttu-id="4bea2-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4bea2-120">Here is a JSON representation of the resource.</span></span>
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



