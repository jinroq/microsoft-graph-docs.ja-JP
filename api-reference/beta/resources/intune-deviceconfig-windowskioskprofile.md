---
title: windowsKioskProfile リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b2ebc01185c9d42cc4dcfd0eae9d3905b1a93c5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370838"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="860f6-103">windowsKioskProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="860f6-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="860f6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="860f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="860f6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="860f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="860f6-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="860f6-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="860f6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="860f6-107">Properties</span></span>
|<span data-ttu-id="860f6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="860f6-108">Property</span></span>|<span data-ttu-id="860f6-109">型</span><span class="sxs-lookup"><span data-stu-id="860f6-109">Type</span></span>|<span data-ttu-id="860f6-110">説明</span><span class="sxs-lookup"><span data-stu-id="860f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="860f6-111">profileId</span><span class="sxs-lookup"><span data-stu-id="860f6-111">profileId</span></span>|<span data-ttu-id="860f6-112">String</span><span class="sxs-lookup"><span data-stu-id="860f6-112">String</span></span>|<span data-ttu-id="860f6-113">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="860f6-113">Key of the entity.</span></span>|
|<span data-ttu-id="860f6-114">profileName</span><span class="sxs-lookup"><span data-stu-id="860f6-114">profileName</span></span>|<span data-ttu-id="860f6-115">String</span><span class="sxs-lookup"><span data-stu-id="860f6-115">String</span></span>|<span data-ttu-id="860f6-116">これは、アプリケーションのグループ、[スタート] メニューにこれらのアプリのレイアウト、およびこのキオスク構成を割り当てるユーザーを識別するために使用されるフレンドリ名です。</span><span class="sxs-lookup"><span data-stu-id="860f6-116">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="860f6-117">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="860f6-117">appConfiguration</span></span>|[<span data-ttu-id="860f6-118">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="860f6-118">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="860f6-119">このキオスク構成で使用されるアプリ構成。</span><span class="sxs-lookup"><span data-stu-id="860f6-119">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="860f6-120">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="860f6-120">userAccountsConfiguration</span></span>|<span data-ttu-id="860f6-121">[Windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="860f6-121">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="860f6-122">このキオスク構成にロックされるユーザーアカウント。</span><span class="sxs-lookup"><span data-stu-id="860f6-122">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="860f6-123">このコレクションには、最大100個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="860f6-123">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="860f6-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="860f6-124">Relationships</span></span>
<span data-ttu-id="860f6-125">なし</span><span class="sxs-lookup"><span data-stu-id="860f6-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="860f6-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="860f6-126">JSON Representation</span></span>
<span data-ttu-id="860f6-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="860f6-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskProfile",
  "profileId": "String",
  "profileName": "String",
  "appConfiguration": {
    "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
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
  },
  "userAccountsConfiguration": [
    {
      "@odata.type": "microsoft.graph.windowsKioskVisitor"
    }
  ]
}
```



