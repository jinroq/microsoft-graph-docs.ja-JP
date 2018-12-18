---
title: iosVppAppAssignmentSettings リソースの種類
description: グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
ms.openlocfilehash: 65a143c1f6cc9eed4dfdc6dabeb6f9379517277c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310249"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="5ba28-103">iosVppAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5ba28-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="5ba28-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ba28-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ba28-105">グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="5ba28-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="5ba28-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="5ba28-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5ba28-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ba28-107">Properties</span></span>
|<span data-ttu-id="5ba28-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ba28-108">Property</span></span>|<span data-ttu-id="5ba28-109">種類</span><span class="sxs-lookup"><span data-stu-id="5ba28-109">Type</span></span>|<span data-ttu-id="5ba28-110">説明</span><span class="sxs-lookup"><span data-stu-id="5ba28-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ba28-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="5ba28-111">useDeviceLicensing</span></span>|<span data-ttu-id="5ba28-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="5ba28-112">Boolean</span></span>|<span data-ttu-id="5ba28-113">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="5ba28-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="5ba28-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="5ba28-114">vpnConfigurationId</span></span>|<span data-ttu-id="5ba28-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5ba28-115">String</span></span>|<span data-ttu-id="5ba28-116">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="5ba28-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ba28-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5ba28-117">Relationships</span></span>
<span data-ttu-id="5ba28-118">なし</span><span class="sxs-lookup"><span data-stu-id="5ba28-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5ba28-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5ba28-119">JSON Representation</span></span>
<span data-ttu-id="5ba28-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5ba28-120">Here is a JSON representation of the resource.</span></span>
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



