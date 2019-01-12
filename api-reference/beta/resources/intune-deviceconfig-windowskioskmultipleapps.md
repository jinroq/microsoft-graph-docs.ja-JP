---
title: windowsKioskMultipleApps リソースの種類
description: キオスクの構成のマルチ ・ モード ・ アプリケーションの構成を識別するために使用するクラス
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3770f8c63be230dff97e43d3706ed35d79826751
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977130"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="c9572-103">windowsKioskMultipleApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9572-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="c9572-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c9572-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9572-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9572-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9572-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c9572-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9572-107">キオスクの構成のマルチ ・ モード ・ アプリケーションの構成を識別するために使用するクラス</span><span class="sxs-lookup"><span data-stu-id="c9572-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>

<span data-ttu-id="c9572-108">[WindowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="c9572-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9572-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9572-109">Properties</span></span>
|<span data-ttu-id="c9572-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9572-110">Property</span></span>|<span data-ttu-id="c9572-111">型</span><span class="sxs-lookup"><span data-stu-id="c9572-111">Type</span></span>|<span data-ttu-id="c9572-112">説明</span><span class="sxs-lookup"><span data-stu-id="c9572-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9572-113">apps</span><span class="sxs-lookup"><span data-stu-id="c9572-113">apps</span></span>|<span data-ttu-id="c9572-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c9572-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="c9572-115">これらは、[スタート] メニューから起動できる唯一の Windows ストア アプリです。</span><span class="sxs-lookup"><span data-stu-id="c9572-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="c9572-116">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="c9572-116">showTaskBar</span></span>|<span data-ttu-id="c9572-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9572-117">Boolean</span></span>|<span data-ttu-id="c9572-118">この設定では、タスク バーを表示するかどうかを指定するのには管理ができます。</span><span class="sxs-lookup"><span data-stu-id="c9572-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="c9572-119">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="c9572-119">disallowDesktopApps</span></span>|<span data-ttu-id="c9572-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9572-120">Boolean</span></span>|<span data-ttu-id="c9572-121">この設定は、デスクトップ アプリケーションを許可することを示します。</span><span class="sxs-lookup"><span data-stu-id="c9572-121">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="c9572-122">デフォルトは true になります。</span><span class="sxs-lookup"><span data-stu-id="c9572-122">Default to true.</span></span>|
|<span data-ttu-id="c9572-123">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="c9572-123">startMenuLayoutXml</span></span>|<span data-ttu-id="c9572-124">Binary</span><span class="sxs-lookup"><span data-stu-id="c9572-124">Binary</span></span>|<span data-ttu-id="c9572-125">開始の既定のレイアウトを変更するのには管理者は、ユーザーが変更できないようにします。</span><span class="sxs-lookup"><span data-stu-id="c9572-125">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="c9572-126">レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="c9572-126"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="c9572-127">XML は、バイナリ形式である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c9572-127">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9572-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c9572-128">Relationships</span></span>
<span data-ttu-id="c9572-129">なし</span><span class="sxs-lookup"><span data-stu-id="c9572-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c9572-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9572-130">JSON Representation</span></span>
<span data-ttu-id="c9572-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c9572-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskMultipleApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskMultipleApps",
  "apps": [
    {
      "@odata.type": "microsoft.graph.windowsKioskUWPApp",
      "startLayoutTileSize": "String",
      "name": "String",
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```





