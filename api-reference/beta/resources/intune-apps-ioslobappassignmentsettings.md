---
title: iosLobAppAssignmentSettings リソースの種類
description: グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f2e0c9ca5b2628343b79ff972e50c3684651c23
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990515"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="28bff-103">iosLobAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="28bff-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="28bff-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="28bff-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28bff-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28bff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28bff-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="28bff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28bff-107">グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。</span><span class="sxs-lookup"><span data-stu-id="28bff-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="28bff-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="28bff-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="28bff-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28bff-109">Properties</span></span>
|<span data-ttu-id="28bff-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28bff-110">Property</span></span>|<span data-ttu-id="28bff-111">種類</span><span class="sxs-lookup"><span data-stu-id="28bff-111">Type</span></span>|<span data-ttu-id="28bff-112">説明</span><span class="sxs-lookup"><span data-stu-id="28bff-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28bff-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="28bff-113">vpnConfigurationId</span></span>|<span data-ttu-id="28bff-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="28bff-114">String</span></span>|<span data-ttu-id="28bff-115">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="28bff-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28bff-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="28bff-116">Relationships</span></span>
<span data-ttu-id="28bff-117">なし</span><span class="sxs-lookup"><span data-stu-id="28bff-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="28bff-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="28bff-118">JSON Representation</span></span>
<span data-ttu-id="28bff-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="28bff-119">Here is a JSON representation of the resource.</span></span>
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





