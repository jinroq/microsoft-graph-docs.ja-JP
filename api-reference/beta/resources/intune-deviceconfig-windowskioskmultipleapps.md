---
title: windowsKioskMultipleApps リソースの種類
description: キオスクの構成のマルチ ・ モード ・ アプリケーションの構成を識別するために使用するクラス
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71b8a57151b08d0297a89dfd815f72d66c2d12a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396029"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="a15a3-103">windowsKioskMultipleApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a15a3-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="a15a3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a15a3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a15a3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a15a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a15a3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a15a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a15a3-107">キオスクの構成のマルチ ・ モード ・ アプリケーションの構成を識別するために使用するクラス</span><span class="sxs-lookup"><span data-stu-id="a15a3-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="a15a3-108">[WindowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a15a3-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a15a3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a15a3-109">Properties</span></span>
|<span data-ttu-id="a15a3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a15a3-110">Property</span></span>|<span data-ttu-id="a15a3-111">型</span><span class="sxs-lookup"><span data-stu-id="a15a3-111">Type</span></span>|<span data-ttu-id="a15a3-112">説明</span><span class="sxs-lookup"><span data-stu-id="a15a3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a15a3-113">apps</span><span class="sxs-lookup"><span data-stu-id="a15a3-113">apps</span></span>|<span data-ttu-id="a15a3-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a15a3-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="a15a3-115">これらは、[スタート] メニューから起動できる唯一の Windows ストア アプリです。</span><span class="sxs-lookup"><span data-stu-id="a15a3-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="a15a3-116">このコレクションは、最大 128 の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a15a3-116">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="a15a3-117">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="a15a3-117">showTaskBar</span></span>|<span data-ttu-id="a15a3-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="a15a3-118">Boolean</span></span>|<span data-ttu-id="a15a3-119">この設定では、タスク バーを表示するかどうかを指定するのには管理ができます。</span><span class="sxs-lookup"><span data-stu-id="a15a3-119">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="a15a3-120">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="a15a3-120">disallowDesktopApps</span></span>|<span data-ttu-id="a15a3-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="a15a3-121">Boolean</span></span>|<span data-ttu-id="a15a3-122">この設定は、デスクトップ アプリケーションを許可することを示します。</span><span class="sxs-lookup"><span data-stu-id="a15a3-122">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="a15a3-123">デフォルトは true になります。</span><span class="sxs-lookup"><span data-stu-id="a15a3-123">Default to true.</span></span>|
|<span data-ttu-id="a15a3-124">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="a15a3-124">startMenuLayoutXml</span></span>|<span data-ttu-id="a15a3-125">Binary</span><span class="sxs-lookup"><span data-stu-id="a15a3-125">Binary</span></span>|<span data-ttu-id="a15a3-126">開始の既定のレイアウトを変更するのには管理者は、ユーザーが変更できないようにします。</span><span class="sxs-lookup"><span data-stu-id="a15a3-126">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="a15a3-127">レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="a15a3-127"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="a15a3-128">XML は、バイナリ形式である必要があります。</span><span class="sxs-lookup"><span data-stu-id="a15a3-128">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a15a3-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a15a3-129">Relationships</span></span>
<span data-ttu-id="a15a3-130">なし</span><span class="sxs-lookup"><span data-stu-id="a15a3-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a15a3-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a15a3-131">JSON Representation</span></span>
<span data-ttu-id="a15a3-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a15a3-132">Here is a JSON representation of the resource.</span></span>
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
      "appType": "String",
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




