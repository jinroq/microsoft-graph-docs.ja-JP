---
title: windowsKioskUWPApp リソースの種類
description: アプリケーションの型の基本クラス
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8719fdd248276a657b96235c592f1bb62607b856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934913"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="792e5-103">windowsKioskUWPApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="792e5-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="792e5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="792e5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="792e5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="792e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="792e5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="792e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="792e5-107">アプリケーションの型の基本クラス</span><span class="sxs-lookup"><span data-stu-id="792e5-107">The base class for a type of apps</span></span>

<span data-ttu-id="792e5-108">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="792e5-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="792e5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="792e5-109">Properties</span></span>
|<span data-ttu-id="792e5-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="792e5-110">Property</span></span>|<span data-ttu-id="792e5-111">種類</span><span class="sxs-lookup"><span data-stu-id="792e5-111">Type</span></span>|<span data-ttu-id="792e5-112">説明</span><span class="sxs-lookup"><span data-stu-id="792e5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="792e5-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="792e5-113">startLayoutTileSize</span></span>|[<span data-ttu-id="792e5-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="792e5-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="792e5-115">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承される開始レイアウトのアプリケーションのタイルのサイズです。</span><span class="sxs-lookup"><span data-stu-id="792e5-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="792e5-116">可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。</span><span class="sxs-lookup"><span data-stu-id="792e5-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="792e5-117">名前</span><span class="sxs-lookup"><span data-stu-id="792e5-117">name</span></span>|<span data-ttu-id="792e5-118">String</span><span class="sxs-lookup"><span data-stu-id="792e5-118">String</span></span>|<span data-ttu-id="792e5-119">[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承される、アプリケーションのフレンドリ名を表す</span><span class="sxs-lookup"><span data-stu-id="792e5-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="792e5-120">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="792e5-120">appUserModelId</span></span>|<span data-ttu-id="792e5-121">String</span><span class="sxs-lookup"><span data-stu-id="792e5-121">String</span></span>|<span data-ttu-id="792e5-122">これは、専用アプリケーション ユーザー モデル ID (AUMID) を表示するキオスク モードでの使用を開始するのには、します。</span><span class="sxs-lookup"><span data-stu-id="792e5-122">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="792e5-123">appId</span><span class="sxs-lookup"><span data-stu-id="792e5-123">appId</span></span>|<span data-ttu-id="792e5-124">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="792e5-124">String</span></span>|<span data-ttu-id="792e5-125">Intune キオスクの構成と同じ割り当ての対象となるアプリケーションを参照してこの</span><span class="sxs-lookup"><span data-stu-id="792e5-125">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="792e5-126">containedAppId</span><span class="sxs-lookup"><span data-stu-id="792e5-126">containedAppId</span></span>|<span data-ttu-id="792e5-127">String</span><span class="sxs-lookup"><span data-stu-id="792e5-127">String</span></span>|<span data-ttu-id="792e5-128">Intune アプリから含まれているアプリケーションを参照してこの</span><span class="sxs-lookup"><span data-stu-id="792e5-128">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="792e5-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="792e5-129">Relationships</span></span>
<span data-ttu-id="792e5-130">なし</span><span class="sxs-lookup"><span data-stu-id="792e5-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="792e5-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="792e5-131">JSON Representation</span></span>
<span data-ttu-id="792e5-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="792e5-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```





