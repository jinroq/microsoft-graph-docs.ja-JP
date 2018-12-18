---
title: windowsKioskSingleUWPApp リソースの種類
description: キオスクの構成の UWP のアプリケーション情報を識別するために使用するクラス
author: tfitzmac
ms.openlocfilehash: fd1dffd5a01b89db27132770d4c8ffe0094eed8f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312181"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="1ec08-103">windowsKioskSingleUWPApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1ec08-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="1ec08-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1ec08-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ec08-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ec08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ec08-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ec08-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ec08-107">キオスクの構成の UWP のアプリケーション情報を識別するために使用するクラス</span><span class="sxs-lookup"><span data-stu-id="1ec08-107">The class used to identify the UWP app info for the kiosk configuration</span></span>

<span data-ttu-id="1ec08-108">[WindowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1ec08-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ec08-109">Properties</span><span class="sxs-lookup"><span data-stu-id="1ec08-109">Properties</span></span>
|<span data-ttu-id="1ec08-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ec08-110">Property</span></span>|<span data-ttu-id="1ec08-111">種類</span><span class="sxs-lookup"><span data-stu-id="1ec08-111">Type</span></span>|<span data-ttu-id="1ec08-112">説明</span><span class="sxs-lookup"><span data-stu-id="1ec08-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ec08-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="1ec08-113">uwpApp</span></span>|[<span data-ttu-id="1ec08-114">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="1ec08-114">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="1ec08-115">これは、専用アプリケーション ユーザー モデル ID (AUMID) を表示するキオスク モードでの使用を開始するのには、します。</span><span class="sxs-lookup"><span data-stu-id="1ec08-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ec08-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1ec08-116">Relationships</span></span>
<span data-ttu-id="1ec08-117">なし</span><span class="sxs-lookup"><span data-stu-id="1ec08-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1ec08-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1ec08-118">JSON Representation</span></span>
<span data-ttu-id="1ec08-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1ec08-119">Here is a JSON representation of the resource.</span></span>
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





