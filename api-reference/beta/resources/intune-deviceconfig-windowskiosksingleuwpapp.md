---
title: windowsKioskSingleUWPApp リソースの種類
description: キオスクの構成の UWP のアプリケーション情報を識別するために使用するクラス
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c11469784e2c450b151c9a81a07f6c1568cf3a3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818145"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="f4e5a-103">windowsKioskSingleUWPApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f4e5a-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="f4e5a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f4e5a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4e5a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4e5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4e5a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f4e5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4e5a-107">キオスクの構成の UWP のアプリケーション情報を識別するために使用するクラス</span><span class="sxs-lookup"><span data-stu-id="f4e5a-107">The class used to identify the UWP app info for the kiosk configuration</span></span>

<span data-ttu-id="f4e5a-108">[WindowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f4e5a-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f4e5a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4e5a-109">Properties</span></span>
|<span data-ttu-id="f4e5a-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4e5a-110">Property</span></span>|<span data-ttu-id="f4e5a-111">種類</span><span class="sxs-lookup"><span data-stu-id="f4e5a-111">Type</span></span>|<span data-ttu-id="f4e5a-112">説明</span><span class="sxs-lookup"><span data-stu-id="f4e5a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4e5a-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="f4e5a-113">uwpApp</span></span>|[<span data-ttu-id="f4e5a-114">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="f4e5a-114">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="f4e5a-115">これは、専用アプリケーション ユーザー モデル ID (AUMID) を表示するキオスク モードでの使用を開始するのには、します。</span><span class="sxs-lookup"><span data-stu-id="f4e5a-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4e5a-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f4e5a-116">Relationships</span></span>
<span data-ttu-id="f4e5a-117">なし</span><span class="sxs-lookup"><span data-stu-id="f4e5a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f4e5a-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4e5a-118">JSON Representation</span></span>
<span data-ttu-id="f4e5a-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f4e5a-119">Here is a JSON representation of the resource.</span></span>
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
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```





