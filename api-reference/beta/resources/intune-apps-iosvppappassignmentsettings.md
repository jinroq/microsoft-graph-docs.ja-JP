---
title: iosVppAppAssignmentSettings リソースの種類
description: グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 77480c88e6fd210704a47f60293081b1ede2e6ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005934"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="a7398-103">iosVppAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a7398-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="a7398-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7398-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7398-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a7398-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7398-106">グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="a7398-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="a7398-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a7398-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a7398-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7398-108">Properties</span></span>
|<span data-ttu-id="a7398-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7398-109">Property</span></span>|<span data-ttu-id="a7398-110">型</span><span class="sxs-lookup"><span data-stu-id="a7398-110">Type</span></span>|<span data-ttu-id="a7398-111">説明</span><span class="sxs-lookup"><span data-stu-id="a7398-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7398-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="a7398-112">useDeviceLicensing</span></span>|<span data-ttu-id="a7398-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="a7398-113">Boolean</span></span>|<span data-ttu-id="a7398-114">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="a7398-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="a7398-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="a7398-115">vpnConfigurationId</span></span>|<span data-ttu-id="a7398-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a7398-116">String</span></span>|<span data-ttu-id="a7398-117">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="a7398-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7398-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a7398-118">Relationships</span></span>
<span data-ttu-id="a7398-119">なし</span><span class="sxs-lookup"><span data-stu-id="a7398-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7398-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a7398-120">JSON Representation</span></span>
<span data-ttu-id="a7398-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a7398-121">Here is a JSON representation of the resource.</span></span>
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





