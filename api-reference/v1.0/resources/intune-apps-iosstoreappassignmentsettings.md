---
title: iosStoreAppAssignmentSettings リソースの種類
description: グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
ms.openlocfilehash: 2f37a4b0cbcacb9e7223793628422fb7bad8a28c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306084"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="d116e-103">iosStoreAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d116e-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="d116e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d116e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d116e-105">グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="d116e-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="d116e-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d116e-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d116e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d116e-107">Properties</span></span>
|<span data-ttu-id="d116e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d116e-108">Property</span></span>|<span data-ttu-id="d116e-109">種類</span><span class="sxs-lookup"><span data-stu-id="d116e-109">Type</span></span>|<span data-ttu-id="d116e-110">説明</span><span class="sxs-lookup"><span data-stu-id="d116e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d116e-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="d116e-111">vpnConfigurationId</span></span>|<span data-ttu-id="d116e-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d116e-112">String</span></span>|<span data-ttu-id="d116e-113">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="d116e-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d116e-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d116e-114">Relationships</span></span>
<span data-ttu-id="d116e-115">なし</span><span class="sxs-lookup"><span data-stu-id="d116e-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d116e-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d116e-116">JSON Representation</span></span>
<span data-ttu-id="d116e-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d116e-117">Here is a JSON representation of the resource.</span></span>
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



