---
title: windowsKioskSingleUWPApp リソースの種類
description: キオスクの構成の UWP アプリ情報を識別するために使用されるクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3bb9c57de0e3e60d1c62adb62c3d1a274c6f853
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793498"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="2b304-103">windowsKioskSingleUWPApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b304-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="2b304-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b304-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b304-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2b304-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b304-106">キオスクの構成の UWP アプリ情報を識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="2b304-106">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="2b304-107">[windowskioskappconfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="2b304-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2b304-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b304-108">Properties</span></span>
|<span data-ttu-id="2b304-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b304-109">Property</span></span>|<span data-ttu-id="2b304-110">型</span><span class="sxs-lookup"><span data-stu-id="2b304-110">Type</span></span>|<span data-ttu-id="2b304-111">説明</span><span class="sxs-lookup"><span data-stu-id="2b304-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b304-112">uwpApp</span><span class="sxs-lookup"><span data-stu-id="2b304-112">uwpApp</span></span>|[<span data-ttu-id="2b304-113">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="2b304-113">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="2b304-114">これは、キオスクモードでの使用が可能になる唯一のアプリケーションユーザーモデル ID (AUMID) です。</span><span class="sxs-lookup"><span data-stu-id="2b304-114">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b304-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2b304-115">Relationships</span></span>
<span data-ttu-id="2b304-116">なし</span><span class="sxs-lookup"><span data-stu-id="2b304-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b304-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b304-117">JSON Representation</span></span>
<span data-ttu-id="2b304-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2b304-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleUWPApp",
  "uwpApp": {
    "@odata.type": "microsoft.graph.windowsKioskUWPApp",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "autoLaunch": true,
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```





