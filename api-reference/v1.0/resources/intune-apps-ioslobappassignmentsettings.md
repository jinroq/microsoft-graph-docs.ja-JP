---
title: iosLobAppAssignmentSettings リソースの種類
description: グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8cb033283c163a30dbedf7088001025c327dbae6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029170"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="c5045-103">iosLobAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c5045-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="c5045-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5045-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5045-105">グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。</span><span class="sxs-lookup"><span data-stu-id="c5045-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="c5045-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c5045-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c5045-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5045-107">Properties</span></span>
|<span data-ttu-id="c5045-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5045-108">Property</span></span>|<span data-ttu-id="c5045-109">型</span><span class="sxs-lookup"><span data-stu-id="c5045-109">Type</span></span>|<span data-ttu-id="c5045-110">説明</span><span class="sxs-lookup"><span data-stu-id="c5045-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5045-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="c5045-111">vpnConfigurationId</span></span>|<span data-ttu-id="c5045-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c5045-112">String</span></span>|<span data-ttu-id="c5045-113">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="c5045-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5045-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c5045-114">Relationships</span></span>
<span data-ttu-id="c5045-115">なし</span><span class="sxs-lookup"><span data-stu-id="c5045-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5045-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c5045-116">JSON Representation</span></span>
<span data-ttu-id="c5045-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c5045-117">Here is a JSON representation of the resource.</span></span>
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



