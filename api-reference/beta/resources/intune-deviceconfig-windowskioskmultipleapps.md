---
title: windowsKioskMultipleApps リソースの種類
description: キオスクの構成のマルチ ・ モード ・ アプリケーションの構成を識別するために使用するクラス
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 01758c66a466b66fcba6b443f80d0350d308756d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851206"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="57850-103">windowsKioskMultipleApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="57850-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="57850-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="57850-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57850-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57850-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57850-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="57850-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57850-107">キオスクの構成のマルチ ・ モード ・ アプリケーションの構成を識別するために使用するクラス</span><span class="sxs-lookup"><span data-stu-id="57850-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>

<span data-ttu-id="57850-108">[WindowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="57850-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="57850-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57850-109">Properties</span></span>
|<span data-ttu-id="57850-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57850-110">Property</span></span>|<span data-ttu-id="57850-111">種類</span><span class="sxs-lookup"><span data-stu-id="57850-111">Type</span></span>|<span data-ttu-id="57850-112">説明</span><span class="sxs-lookup"><span data-stu-id="57850-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57850-113">apps</span><span class="sxs-lookup"><span data-stu-id="57850-113">apps</span></span>|<span data-ttu-id="57850-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="57850-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="57850-115">これらは、[スタート] メニューから起動できる唯一の Windows ストア アプリです。</span><span class="sxs-lookup"><span data-stu-id="57850-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="57850-116">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="57850-116">showTaskBar</span></span>|<span data-ttu-id="57850-117">ブール型</span><span class="sxs-lookup"><span data-stu-id="57850-117">Boolean</span></span>|<span data-ttu-id="57850-118">この設定では、タスク バーを表示するかどうかを指定するのには管理ができます。</span><span class="sxs-lookup"><span data-stu-id="57850-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="57850-119">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="57850-119">disallowDesktopApps</span></span>|<span data-ttu-id="57850-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="57850-120">Boolean</span></span>|<span data-ttu-id="57850-121">この設定は、デスクトップ アプリケーションを許可することを示します。</span><span class="sxs-lookup"><span data-stu-id="57850-121">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="57850-122">デフォルトは true になります。</span><span class="sxs-lookup"><span data-stu-id="57850-122">Default to true.</span></span>|
|<span data-ttu-id="57850-123">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="57850-123">startMenuLayoutXml</span></span>|<span data-ttu-id="57850-124">Binary</span><span class="sxs-lookup"><span data-stu-id="57850-124">Binary</span></span>|<span data-ttu-id="57850-125">開始の既定のレイアウトを変更するのには管理者は、ユーザーが変更できないようにします。</span><span class="sxs-lookup"><span data-stu-id="57850-125">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="57850-126">レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="57850-126"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="57850-127">XML は、バイナリ形式である必要があります。</span><span class="sxs-lookup"><span data-stu-id="57850-127">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57850-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="57850-128">Relationships</span></span>
<span data-ttu-id="57850-129">なし</span><span class="sxs-lookup"><span data-stu-id="57850-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="57850-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="57850-130">JSON Representation</span></span>
<span data-ttu-id="57850-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="57850-131">Here is a JSON representation of the resource.</span></span>
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





