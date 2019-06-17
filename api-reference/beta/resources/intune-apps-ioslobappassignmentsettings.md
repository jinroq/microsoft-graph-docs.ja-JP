---
title: iosLobAppAssignmentSettings リソースの種類
description: グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c27321490cca54a912a5956026706e1d9b48d1d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991171"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="30755-103">iosLobAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="30755-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="30755-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30755-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30755-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="30755-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30755-106">グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。</span><span class="sxs-lookup"><span data-stu-id="30755-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="30755-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="30755-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="30755-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30755-108">Properties</span></span>
|<span data-ttu-id="30755-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30755-109">Property</span></span>|<span data-ttu-id="30755-110">型</span><span class="sxs-lookup"><span data-stu-id="30755-110">Type</span></span>|<span data-ttu-id="30755-111">説明</span><span class="sxs-lookup"><span data-stu-id="30755-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30755-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="30755-112">vpnConfigurationId</span></span>|<span data-ttu-id="30755-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="30755-113">String</span></span>|<span data-ttu-id="30755-114">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="30755-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30755-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="30755-115">Relationships</span></span>
<span data-ttu-id="30755-116">なし</span><span class="sxs-lookup"><span data-stu-id="30755-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30755-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="30755-117">JSON Representation</span></span>
<span data-ttu-id="30755-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="30755-118">Here is a JSON representation of the resource.</span></span>
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





