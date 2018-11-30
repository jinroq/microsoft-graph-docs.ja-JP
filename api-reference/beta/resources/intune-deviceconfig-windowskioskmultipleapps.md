---
title: windowsKioskMultipleApps リソースの種類
description: キオスクの構成のマルチ ・ モード ・ アプリケーションの構成を識別するために使用するクラス
ms.openlocfilehash: 2b52cbe343c4a8d81391ad448e8f10f64fef295e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069116"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="65a5f-103">windowsKioskMultipleApps リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65a5f-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="65a5f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="65a5f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65a5f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65a5f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65a5f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="65a5f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65a5f-107">キオスクの構成のマルチ ・ モード ・ アプリケーションの構成を識別するために使用するクラス</span><span class="sxs-lookup"><span data-stu-id="65a5f-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>

<span data-ttu-id="65a5f-108">[WindowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="65a5f-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="65a5f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65a5f-109">Properties</span></span>
|<span data-ttu-id="65a5f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65a5f-110">Property</span></span>|<span data-ttu-id="65a5f-111">型</span><span class="sxs-lookup"><span data-stu-id="65a5f-111">Type</span></span>|<span data-ttu-id="65a5f-112">説明</span><span class="sxs-lookup"><span data-stu-id="65a5f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65a5f-113">apps</span><span class="sxs-lookup"><span data-stu-id="65a5f-113">apps</span></span>|<span data-ttu-id="65a5f-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="65a5f-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="65a5f-115">これらは、[スタート] メニューから起動できる唯一の Windows ストア アプリです。</span><span class="sxs-lookup"><span data-stu-id="65a5f-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="65a5f-116">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="65a5f-116">showTaskBar</span></span>|<span data-ttu-id="65a5f-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="65a5f-117">Boolean</span></span>|<span data-ttu-id="65a5f-118">この設定では、タスク バーを表示するかどうかを指定するのには管理ができます。</span><span class="sxs-lookup"><span data-stu-id="65a5f-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="65a5f-119">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="65a5f-119">disallowDesktopApps</span></span>|<span data-ttu-id="65a5f-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="65a5f-120">Boolean</span></span>|<span data-ttu-id="65a5f-121">この設定は、デスクトップ アプリケーションを許可することを示します。</span><span class="sxs-lookup"><span data-stu-id="65a5f-121">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="65a5f-122">デフォルトは true になります。</span><span class="sxs-lookup"><span data-stu-id="65a5f-122">Default to true.</span></span>|
|<span data-ttu-id="65a5f-123">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="65a5f-123">startMenuLayoutXml</span></span>|<span data-ttu-id="65a5f-124">Binary</span><span class="sxs-lookup"><span data-stu-id="65a5f-124">Binary</span></span>|<span data-ttu-id="65a5f-125">開始の既定のレイアウトを変更するのには管理者は、ユーザーが変更できないようにします。</span><span class="sxs-lookup"><span data-stu-id="65a5f-125">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="65a5f-126">レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="65a5f-126"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="65a5f-127">XML は、バイナリ形式である必要があります。</span><span class="sxs-lookup"><span data-stu-id="65a5f-127">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65a5f-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65a5f-128">Relationships</span></span>
<span data-ttu-id="65a5f-129">なし</span><span class="sxs-lookup"><span data-stu-id="65a5f-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="65a5f-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65a5f-130">JSON Representation</span></span>
<span data-ttu-id="65a5f-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65a5f-131">Here is a JSON representation of the resource.</span></span>
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





