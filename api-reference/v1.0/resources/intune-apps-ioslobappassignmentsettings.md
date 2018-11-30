---
title: iosLobAppAssignmentSettings リソースの種類
description: グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。
ms.openlocfilehash: 29642e7ba4d834d4481d5bc04b0d82a7046f544d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023652"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="66258-103">iosLobAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66258-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="66258-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="66258-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66258-105">グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。</span><span class="sxs-lookup"><span data-stu-id="66258-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="66258-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="66258-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="66258-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66258-107">Properties</span></span>
|<span data-ttu-id="66258-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66258-108">Property</span></span>|<span data-ttu-id="66258-109">型</span><span class="sxs-lookup"><span data-stu-id="66258-109">Type</span></span>|<span data-ttu-id="66258-110">説明</span><span class="sxs-lookup"><span data-stu-id="66258-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66258-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="66258-111">vpnConfigurationId</span></span>|<span data-ttu-id="66258-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="66258-112">String</span></span>|<span data-ttu-id="66258-113">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="66258-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66258-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="66258-114">Relationships</span></span>
<span data-ttu-id="66258-115">なし</span><span class="sxs-lookup"><span data-stu-id="66258-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="66258-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66258-116">JSON Representation</span></span>
<span data-ttu-id="66258-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="66258-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



