---
title: iosStoreAppAssignmentSettings リソースの種類
description: グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da1d42d092c7a85831da6ae26b55b43db7ac7db7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365988"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="f108b-103">iosStoreAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f108b-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="f108b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f108b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f108b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f108b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f108b-106">グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="f108b-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="f108b-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f108b-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f108b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f108b-108">Properties</span></span>
|<span data-ttu-id="f108b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f108b-109">Property</span></span>|<span data-ttu-id="f108b-110">型</span><span class="sxs-lookup"><span data-stu-id="f108b-110">Type</span></span>|<span data-ttu-id="f108b-111">説明</span><span class="sxs-lookup"><span data-stu-id="f108b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f108b-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f108b-112">vpnConfigurationId</span></span>|<span data-ttu-id="f108b-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f108b-113">String</span></span>|<span data-ttu-id="f108b-114">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="f108b-114">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="f108b-115">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="f108b-115">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="f108b-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="f108b-116">Boolean</span></span>|<span data-ttu-id="f108b-117">デバイスが Intune から削除されたときにアプリをアンインストールするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f108b-117">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f108b-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f108b-118">Relationships</span></span>
<span data-ttu-id="f108b-119">なし</span><span class="sxs-lookup"><span data-stu-id="f108b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f108b-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f108b-120">JSON Representation</span></span>
<span data-ttu-id="f108b-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f108b-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```



