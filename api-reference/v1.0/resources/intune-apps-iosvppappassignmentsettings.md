---
title: iosVppAppAssignmentSettings リソースの種類
description: グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e221ceb67789f9d96195a31bd7eba8f37a9df6bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917644"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="1e17c-103">iosVppAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e17c-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1e17c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e17c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e17c-105">グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="1e17c-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="1e17c-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="1e17c-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1e17c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e17c-107">Properties</span></span>
|<span data-ttu-id="1e17c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e17c-108">Property</span></span>|<span data-ttu-id="1e17c-109">種類</span><span class="sxs-lookup"><span data-stu-id="1e17c-109">Type</span></span>|<span data-ttu-id="1e17c-110">説明</span><span class="sxs-lookup"><span data-stu-id="1e17c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e17c-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="1e17c-111">useDeviceLicensing</span></span>|<span data-ttu-id="1e17c-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1e17c-112">Boolean</span></span>|<span data-ttu-id="1e17c-113">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="1e17c-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="1e17c-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="1e17c-114">vpnConfigurationId</span></span>|<span data-ttu-id="1e17c-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1e17c-115">String</span></span>|<span data-ttu-id="1e17c-116">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="1e17c-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e17c-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1e17c-117">Relationships</span></span>
<span data-ttu-id="1e17c-118">なし</span><span class="sxs-lookup"><span data-stu-id="1e17c-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1e17c-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e17c-119">JSON Representation</span></span>
<span data-ttu-id="1e17c-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1e17c-120">Here is a JSON representation of the resource.</span></span>
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



