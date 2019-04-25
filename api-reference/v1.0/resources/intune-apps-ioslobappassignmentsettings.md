---
title: iosLobAppAssignmentSettings リソースの種類
description: グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5beacfd60eb2237ed85a95bca21c27a38f956d16
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583159"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="5ad26-103">iosLobAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5ad26-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="5ad26-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5ad26-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ad26-105">グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。</span><span class="sxs-lookup"><span data-stu-id="5ad26-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="5ad26-106">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="5ad26-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5ad26-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ad26-107">Properties</span></span>
|<span data-ttu-id="5ad26-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ad26-108">Property</span></span>|<span data-ttu-id="5ad26-109">型</span><span class="sxs-lookup"><span data-stu-id="5ad26-109">Type</span></span>|<span data-ttu-id="5ad26-110">説明</span><span class="sxs-lookup"><span data-stu-id="5ad26-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ad26-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="5ad26-111">vpnConfigurationId</span></span>|<span data-ttu-id="5ad26-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5ad26-112">String</span></span>|<span data-ttu-id="5ad26-113">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="5ad26-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ad26-114">関係</span><span class="sxs-lookup"><span data-stu-id="5ad26-114">Relationships</span></span>
<span data-ttu-id="5ad26-115">なし</span><span class="sxs-lookup"><span data-stu-id="5ad26-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ad26-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5ad26-116">JSON Representation</span></span>
<span data-ttu-id="5ad26-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5ad26-117">Here is a JSON representation of the resource.</span></span>
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



