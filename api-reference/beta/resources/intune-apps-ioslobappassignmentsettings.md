---
title: iosLobAppAssignmentSettings リソースの種類
description: グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3cb8c437d5cb943ef4d6f76ed515b917f8a3e10a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366064"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="d4f32-103">iosLobAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d4f32-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="d4f32-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4f32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4f32-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4f32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4f32-106">グループへの iOS LOB モバイル アプリの割り当てに使用されるプロパティが、含まれます。</span><span class="sxs-lookup"><span data-stu-id="d4f32-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="d4f32-107">[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d4f32-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d4f32-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4f32-108">Properties</span></span>
|<span data-ttu-id="d4f32-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4f32-109">Property</span></span>|<span data-ttu-id="d4f32-110">型</span><span class="sxs-lookup"><span data-stu-id="d4f32-110">Type</span></span>|<span data-ttu-id="d4f32-111">説明</span><span class="sxs-lookup"><span data-stu-id="d4f32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4f32-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="d4f32-112">vpnConfigurationId</span></span>|<span data-ttu-id="d4f32-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d4f32-113">String</span></span>|<span data-ttu-id="d4f32-114">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="d4f32-114">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="d4f32-115">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="d4f32-115">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="d4f32-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4f32-116">Boolean</span></span>|<span data-ttu-id="d4f32-117">デバイスが Intune から削除されたときにアプリをアンインストールするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d4f32-117">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4f32-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d4f32-118">Relationships</span></span>
<span data-ttu-id="d4f32-119">なし</span><span class="sxs-lookup"><span data-stu-id="d4f32-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4f32-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d4f32-120">JSON Representation</span></span>
<span data-ttu-id="d4f32-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d4f32-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```



