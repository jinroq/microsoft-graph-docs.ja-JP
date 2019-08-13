---
title: windowsKioskSingleUWPApp リソースの種類
description: キオスクの構成の UWP アプリ情報を識別するために使用されるクラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 87e73eed445d3160cfbfcab8f0a7abe00a27139d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370817"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="499d3-103">windowsKioskSingleUWPApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="499d3-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="499d3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="499d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="499d3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="499d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="499d3-106">キオスクの構成の UWP アプリ情報を識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="499d3-106">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="499d3-107">[Windowskioskappconfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="499d3-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="499d3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="499d3-108">Properties</span></span>
|<span data-ttu-id="499d3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="499d3-109">Property</span></span>|<span data-ttu-id="499d3-110">型</span><span class="sxs-lookup"><span data-stu-id="499d3-110">Type</span></span>|<span data-ttu-id="499d3-111">説明</span><span class="sxs-lookup"><span data-stu-id="499d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="499d3-112">uwpApp</span><span class="sxs-lookup"><span data-stu-id="499d3-112">uwpApp</span></span>|[<span data-ttu-id="499d3-113">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="499d3-113">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="499d3-114">これは、キオスクモードでの使用が可能になる唯一のアプリケーションユーザーモデル ID (AUMID) です。</span><span class="sxs-lookup"><span data-stu-id="499d3-114">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="499d3-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="499d3-115">Relationships</span></span>
<span data-ttu-id="499d3-116">なし</span><span class="sxs-lookup"><span data-stu-id="499d3-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="499d3-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="499d3-117">JSON Representation</span></span>
<span data-ttu-id="499d3-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="499d3-118">Here is a JSON representation of the resource.</span></span>
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



