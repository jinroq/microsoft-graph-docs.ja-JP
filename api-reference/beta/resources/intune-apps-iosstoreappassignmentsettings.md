---
title: iosStoreAppAssignmentSettings リソースの種類
description: グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 311b7469b0002dcf12369e650066e4e0b08ac83f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856531"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="0a214-103">iosStoreAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a214-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="0a214-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0a214-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a214-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a214-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a214-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a214-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a214-107">グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="0a214-107">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="0a214-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0a214-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0a214-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a214-109">Properties</span></span>
|<span data-ttu-id="0a214-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a214-110">Property</span></span>|<span data-ttu-id="0a214-111">種類</span><span class="sxs-lookup"><span data-stu-id="0a214-111">Type</span></span>|<span data-ttu-id="0a214-112">説明</span><span class="sxs-lookup"><span data-stu-id="0a214-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a214-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="0a214-113">vpnConfigurationId</span></span>|<span data-ttu-id="0a214-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0a214-114">String</span></span>|<span data-ttu-id="0a214-115">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="0a214-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a214-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0a214-116">Relationships</span></span>
<span data-ttu-id="0a214-117">なし</span><span class="sxs-lookup"><span data-stu-id="0a214-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0a214-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a214-118">JSON Representation</span></span>
<span data-ttu-id="0a214-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a214-119">Here is a JSON representation of the resource.</span></span>
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





