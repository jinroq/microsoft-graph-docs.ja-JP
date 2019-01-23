---
title: iosLobAppAssignmentSettings リソースの種類
description: グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4f2d954b016ed2a59938974f995d9bd040bc69b1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404352"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="c7859-103">iosLobAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7859-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="c7859-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c7859-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c7859-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7859-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7859-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c7859-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7859-107">グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。</span><span class="sxs-lookup"><span data-stu-id="c7859-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="c7859-108">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c7859-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7859-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7859-109">Properties</span></span>
|<span data-ttu-id="c7859-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7859-110">Property</span></span>|<span data-ttu-id="c7859-111">型</span><span class="sxs-lookup"><span data-stu-id="c7859-111">Type</span></span>|<span data-ttu-id="c7859-112">説明</span><span class="sxs-lookup"><span data-stu-id="c7859-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7859-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="c7859-113">vpnConfigurationId</span></span>|<span data-ttu-id="c7859-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c7859-114">String</span></span>|<span data-ttu-id="c7859-115">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="c7859-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7859-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c7859-116">Relationships</span></span>
<span data-ttu-id="c7859-117">なし</span><span class="sxs-lookup"><span data-stu-id="c7859-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7859-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7859-118">JSON Representation</span></span>
<span data-ttu-id="c7859-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c7859-119">Here is a JSON representation of the resource.</span></span>
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




