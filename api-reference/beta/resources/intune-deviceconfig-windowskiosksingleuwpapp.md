---
title: windowsKioskSingleUWPApp リソースの種類
description: キオスクの構成の UWP のアプリケーション情報を識別するために使用するクラス
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e62dc6393cc2dc6a9133732a42527abdfadbd91e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409378"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="d757a-103">windowsKioskSingleUWPApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d757a-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="d757a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d757a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d757a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d757a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d757a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d757a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d757a-107">キオスクの構成の UWP のアプリケーション情報を識別するために使用するクラス</span><span class="sxs-lookup"><span data-stu-id="d757a-107">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="d757a-108">[WindowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d757a-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d757a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d757a-109">Properties</span></span>
|<span data-ttu-id="d757a-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d757a-110">Property</span></span>|<span data-ttu-id="d757a-111">型</span><span class="sxs-lookup"><span data-stu-id="d757a-111">Type</span></span>|<span data-ttu-id="d757a-112">説明</span><span class="sxs-lookup"><span data-stu-id="d757a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d757a-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="d757a-113">uwpApp</span></span>|[<span data-ttu-id="d757a-114">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="d757a-114">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="d757a-115">これは、専用アプリケーション ユーザー モデル ID (AUMID) を表示するキオスク モードでの使用を開始するのには、します。</span><span class="sxs-lookup"><span data-stu-id="d757a-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="d757a-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d757a-116">Relationships</span></span>
<span data-ttu-id="d757a-117">なし</span><span class="sxs-lookup"><span data-stu-id="d757a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d757a-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d757a-118">JSON Representation</span></span>
<span data-ttu-id="d757a-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d757a-119">Here is a JSON representation of the resource.</span></span>
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
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```




