---
title: iosStoreAppAssignmentSettings リソースの種類
description: グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。
ms.openlocfilehash: 5509227dd28d7d89c9afcd8c6abeb89db6096ddf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071087"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="4fc09-103">iosStoreAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4fc09-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="4fc09-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4fc09-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4fc09-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fc09-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4fc09-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4fc09-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4fc09-107">グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="4fc09-107">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="4fc09-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4fc09-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4fc09-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fc09-109">Properties</span></span>
|<span data-ttu-id="4fc09-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fc09-110">Property</span></span>|<span data-ttu-id="4fc09-111">型</span><span class="sxs-lookup"><span data-stu-id="4fc09-111">Type</span></span>|<span data-ttu-id="4fc09-112">説明</span><span class="sxs-lookup"><span data-stu-id="4fc09-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fc09-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="4fc09-113">vpnConfigurationId</span></span>|<span data-ttu-id="4fc09-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4fc09-114">String</span></span>|<span data-ttu-id="4fc09-115">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="4fc09-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fc09-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4fc09-116">Relationships</span></span>
<span data-ttu-id="4fc09-117">なし</span><span class="sxs-lookup"><span data-stu-id="4fc09-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4fc09-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4fc09-118">JSON Representation</span></span>
<span data-ttu-id="4fc09-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4fc09-119">Here is a JSON representation of the resource.</span></span>
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





