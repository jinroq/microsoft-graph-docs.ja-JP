---
title: iosVppAppAssignmentSettings リソースの種類
description: グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2dd3f8816aaa4e08066e329e4a9f4630e3f27f1d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867768"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="8a41c-103">iosVppAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a41c-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="8a41c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8a41c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a41c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a41c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a41c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a41c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a41c-107">グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="8a41c-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="8a41c-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8a41c-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8a41c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a41c-109">Properties</span></span>
|<span data-ttu-id="8a41c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a41c-110">Property</span></span>|<span data-ttu-id="8a41c-111">種類</span><span class="sxs-lookup"><span data-stu-id="8a41c-111">Type</span></span>|<span data-ttu-id="8a41c-112">説明</span><span class="sxs-lookup"><span data-stu-id="8a41c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a41c-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="8a41c-113">useDeviceLicensing</span></span>|<span data-ttu-id="8a41c-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8a41c-114">Boolean</span></span>|<span data-ttu-id="8a41c-115">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="8a41c-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="8a41c-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="8a41c-116">vpnConfigurationId</span></span>|<span data-ttu-id="8a41c-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8a41c-117">String</span></span>|<span data-ttu-id="8a41c-118">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="8a41c-118">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a41c-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a41c-119">Relationships</span></span>
<span data-ttu-id="8a41c-120">なし</span><span class="sxs-lookup"><span data-stu-id="8a41c-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8a41c-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a41c-121">JSON Representation</span></span>
<span data-ttu-id="8a41c-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8a41c-122">Here is a JSON representation of the resource.</span></span>
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





