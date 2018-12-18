---
title: iosLobAppAssignmentSettings リソースの種類
description: グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。
author: tfitzmac
ms.openlocfilehash: ca85fff558285ea52f14e359d17511a3e879e24a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361741"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="65945-103">iosLobAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65945-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="65945-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="65945-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65945-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65945-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65945-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="65945-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65945-107">グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。</span><span class="sxs-lookup"><span data-stu-id="65945-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="65945-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="65945-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="65945-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65945-109">Properties</span></span>
|<span data-ttu-id="65945-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65945-110">Property</span></span>|<span data-ttu-id="65945-111">種類</span><span class="sxs-lookup"><span data-stu-id="65945-111">Type</span></span>|<span data-ttu-id="65945-112">説明</span><span class="sxs-lookup"><span data-stu-id="65945-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65945-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="65945-113">vpnConfigurationId</span></span>|<span data-ttu-id="65945-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="65945-114">String</span></span>|<span data-ttu-id="65945-115">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="65945-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65945-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65945-116">Relationships</span></span>
<span data-ttu-id="65945-117">なし</span><span class="sxs-lookup"><span data-stu-id="65945-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="65945-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65945-118">JSON Representation</span></span>
<span data-ttu-id="65945-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65945-119">Here is a JSON representation of the resource.</span></span>
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





