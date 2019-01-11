---
title: iosStoreAppAssignmentSettings リソースの種類
description: グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 34776d6002926486baa05d0720ce1c7eeecee927
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822233"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="d9e84-103">iosStoreAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d9e84-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="d9e84-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d9e84-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9e84-105">グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="d9e84-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="d9e84-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d9e84-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d9e84-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9e84-107">Properties</span></span>
|<span data-ttu-id="d9e84-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9e84-108">Property</span></span>|<span data-ttu-id="d9e84-109">種類</span><span class="sxs-lookup"><span data-stu-id="d9e84-109">Type</span></span>|<span data-ttu-id="d9e84-110">説明</span><span class="sxs-lookup"><span data-stu-id="d9e84-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9e84-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="d9e84-111">vpnConfigurationId</span></span>|<span data-ttu-id="d9e84-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d9e84-112">String</span></span>|<span data-ttu-id="d9e84-113">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="d9e84-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9e84-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d9e84-114">Relationships</span></span>
<span data-ttu-id="d9e84-115">なし</span><span class="sxs-lookup"><span data-stu-id="d9e84-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d9e84-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d9e84-116">JSON Representation</span></span>
<span data-ttu-id="d9e84-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d9e84-117">Here is a JSON representation of the resource.</span></span>
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



