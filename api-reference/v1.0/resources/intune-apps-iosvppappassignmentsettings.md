---
title: iosVppAppAssignmentSettings リソースの種類
description: グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。
ms.openlocfilehash: 6fc529fe1aeea6bdbef46ad0cd97fb5830250b4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023265"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="bb3b9-103">iosVppAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb3b9-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="bb3b9-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bb3b9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb3b9-105">グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="bb3b9-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="bb3b9-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bb3b9-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bb3b9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb3b9-107">Properties</span></span>
|<span data-ttu-id="bb3b9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb3b9-108">Property</span></span>|<span data-ttu-id="bb3b9-109">型</span><span class="sxs-lookup"><span data-stu-id="bb3b9-109">Type</span></span>|<span data-ttu-id="bb3b9-110">説明</span><span class="sxs-lookup"><span data-stu-id="bb3b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb3b9-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="bb3b9-111">useDeviceLicensing</span></span>|<span data-ttu-id="bb3b9-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="bb3b9-112">Boolean</span></span>|<span data-ttu-id="bb3b9-113">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="bb3b9-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="bb3b9-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="bb3b9-114">vpnConfigurationId</span></span>|<span data-ttu-id="bb3b9-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bb3b9-115">String</span></span>|<span data-ttu-id="bb3b9-116">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="bb3b9-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb3b9-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb3b9-117">Relationships</span></span>
<span data-ttu-id="bb3b9-118">なし</span><span class="sxs-lookup"><span data-stu-id="bb3b9-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bb3b9-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb3b9-119">JSON Representation</span></span>
<span data-ttu-id="bb3b9-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb3b9-120">Here is a JSON representation of the resource.</span></span>
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



