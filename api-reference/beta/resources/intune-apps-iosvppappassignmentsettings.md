---
title: iosVppAppAssignmentSettings リソースの種類
description: グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36c6e2c60423038f2af10ccdbcfaf94ecd6ec3aa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552325"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="3f47a-103">iosVppAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3f47a-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="3f47a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f47a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f47a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3f47a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f47a-106">グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="3f47a-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="3f47a-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="3f47a-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3f47a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f47a-108">Properties</span></span>
|<span data-ttu-id="3f47a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f47a-109">Property</span></span>|<span data-ttu-id="3f47a-110">型</span><span class="sxs-lookup"><span data-stu-id="3f47a-110">Type</span></span>|<span data-ttu-id="3f47a-111">説明</span><span class="sxs-lookup"><span data-stu-id="3f47a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f47a-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="3f47a-112">useDeviceLicensing</span></span>|<span data-ttu-id="3f47a-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="3f47a-113">Boolean</span></span>|<span data-ttu-id="3f47a-114">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="3f47a-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="3f47a-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="3f47a-115">vpnConfigurationId</span></span>|<span data-ttu-id="3f47a-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3f47a-116">String</span></span>|<span data-ttu-id="3f47a-117">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="3f47a-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f47a-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3f47a-118">Relationships</span></span>
<span data-ttu-id="3f47a-119">なし</span><span class="sxs-lookup"><span data-stu-id="3f47a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f47a-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3f47a-120">JSON Representation</span></span>
<span data-ttu-id="3f47a-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3f47a-121">Here is a JSON representation of the resource.</span></span>
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





