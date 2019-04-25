---
title: windowskiosk多重アプリリソースの種類
description: キオスク構成でのマルチモードアプリの構成を識別するために使用されるクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cae99ce452cdb9b002ebe4fe24968ec368c9fc0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574517"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="ddb4b-103">windowskiosk多重アプリリソースの種類</span><span class="sxs-lookup"><span data-stu-id="ddb4b-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="ddb4b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddb4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddb4b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ddb4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddb4b-106">キオスク構成でのマルチモードアプリの構成を識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="ddb4b-106">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="ddb4b-107">[windowskioskappconfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="ddb4b-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ddb4b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddb4b-108">Properties</span></span>
|<span data-ttu-id="ddb4b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddb4b-109">Property</span></span>|<span data-ttu-id="ddb4b-110">型</span><span class="sxs-lookup"><span data-stu-id="ddb4b-110">Type</span></span>|<span data-ttu-id="ddb4b-111">説明</span><span class="sxs-lookup"><span data-stu-id="ddb4b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddb4b-112">apps</span><span class="sxs-lookup"><span data-stu-id="ddb4b-112">apps</span></span>|<span data-ttu-id="ddb4b-113">[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ddb4b-113">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="ddb4b-114">[スタート] メニューから起動できる Windows ストアアプリは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ddb4b-114">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="ddb4b-115">このコレクションには、最大128個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ddb4b-115">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="ddb4b-116">showtaskbar バー</span><span class="sxs-lookup"><span data-stu-id="ddb4b-116">showTaskBar</span></span>|<span data-ttu-id="ddb4b-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb4b-117">Boolean</span></span>|<span data-ttu-id="ddb4b-118">この設定では、管理者がタスクバーを表示するかどうかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="ddb4b-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="ddb4b-119">allowAccessToDownloadsFolder</span><span class="sxs-lookup"><span data-stu-id="ddb4b-119">allowAccessToDownloadsFolder</span></span>|<span data-ttu-id="ddb4b-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb4b-120">Boolean</span></span>|<span data-ttu-id="ddb4b-121">この設定では、エクスプローラーの [ダウンロード] フォルダーにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="ddb4b-121">This setting allows access to Downloads folder in file explorer.</span></span>|
|<span data-ttu-id="ddb4b-122">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="ddb4b-122">disallowDesktopApps</span></span>|<span data-ttu-id="ddb4b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb4b-123">Boolean</span></span>|<span data-ttu-id="ddb4b-124">この設定は、デスクトップアプリが許可されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="ddb4b-124">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="ddb4b-125">既定値は true です。</span><span class="sxs-lookup"><span data-stu-id="ddb4b-125">Default to true.</span></span>|
|<span data-ttu-id="ddb4b-126">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="ddb4b-126">startMenuLayoutXml</span></span>|<span data-ttu-id="ddb4b-127">Binary</span><span class="sxs-lookup"><span data-stu-id="ddb4b-127">Binary</span></span>|<span data-ttu-id="ddb4b-128">管理者が既定の開始レイアウトを上書きし、ユーザーがそれを変更できないようにします。</span><span class="sxs-lookup"><span data-stu-id="ddb4b-128">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="ddb4b-129">レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="ddb4b-129"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="ddb4b-130">XML はバイナリ形式である必要があります。</span><span class="sxs-lookup"><span data-stu-id="ddb4b-130">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddb4b-131">関係</span><span class="sxs-lookup"><span data-stu-id="ddb4b-131">Relationships</span></span>
<span data-ttu-id="ddb4b-132">なし</span><span class="sxs-lookup"><span data-stu-id="ddb4b-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddb4b-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ddb4b-133">JSON Representation</span></span>
<span data-ttu-id="ddb4b-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ddb4b-134">Here is a JSON representation of the resource.</span></span>
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
      "autoLaunch": true,
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "allowAccessToDownloadsFolder": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```





