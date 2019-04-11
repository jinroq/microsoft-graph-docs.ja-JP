---
title: iosStoreAppAssignmentSettings リソースの種類
description: グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcda842b97c6c7baf257145f0333c6194e97a403
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806427"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="aaa1a-103">iosStoreAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aaa1a-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="aaa1a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aaa1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaa1a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aaa1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaa1a-106">グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="aaa1a-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="aaa1a-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="aaa1a-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aaa1a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aaa1a-108">Properties</span></span>
|<span data-ttu-id="aaa1a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aaa1a-109">Property</span></span>|<span data-ttu-id="aaa1a-110">型</span><span class="sxs-lookup"><span data-stu-id="aaa1a-110">Type</span></span>|<span data-ttu-id="aaa1a-111">説明</span><span class="sxs-lookup"><span data-stu-id="aaa1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaa1a-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="aaa1a-112">vpnConfigurationId</span></span>|<span data-ttu-id="aaa1a-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="aaa1a-113">String</span></span>|<span data-ttu-id="aaa1a-114">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="aaa1a-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aaa1a-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aaa1a-115">Relationships</span></span>
<span data-ttu-id="aaa1a-116">なし</span><span class="sxs-lookup"><span data-stu-id="aaa1a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aaa1a-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aaa1a-117">JSON Representation</span></span>
<span data-ttu-id="aaa1a-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aaa1a-118">Here is a JSON representation of the resource.</span></span>
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





