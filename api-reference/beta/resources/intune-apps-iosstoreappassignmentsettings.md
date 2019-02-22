---
title: iosStoreAppAssignmentSettings リソースの種類
description: グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d700b6a736f7d4a33362a66aeb8b75e6df7c605
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153964"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="b69e5-103">iosStoreAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b69e5-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="b69e5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b69e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b69e5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b69e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b69e5-106">グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="b69e5-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="b69e5-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b69e5-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b69e5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b69e5-108">Properties</span></span>
|<span data-ttu-id="b69e5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b69e5-109">Property</span></span>|<span data-ttu-id="b69e5-110">型</span><span class="sxs-lookup"><span data-stu-id="b69e5-110">Type</span></span>|<span data-ttu-id="b69e5-111">説明</span><span class="sxs-lookup"><span data-stu-id="b69e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b69e5-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="b69e5-112">vpnConfigurationId</span></span>|<span data-ttu-id="b69e5-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b69e5-113">String</span></span>|<span data-ttu-id="b69e5-114">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="b69e5-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b69e5-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b69e5-115">Relationships</span></span>
<span data-ttu-id="b69e5-116">なし</span><span class="sxs-lookup"><span data-stu-id="b69e5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b69e5-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b69e5-117">JSON Representation</span></span>
<span data-ttu-id="b69e5-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b69e5-118">Here is a JSON representation of the resource.</span></span>
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




