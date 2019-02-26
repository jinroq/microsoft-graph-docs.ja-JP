---
title: windowskioskprofile リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1c7107982a33452cd9dd00829cba08f108c6394
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164751"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="715ee-103">windowskioskprofile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="715ee-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="715ee-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="715ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="715ee-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="715ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="715ee-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="715ee-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="715ee-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="715ee-107">Properties</span></span>
|<span data-ttu-id="715ee-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="715ee-108">Property</span></span>|<span data-ttu-id="715ee-109">型</span><span class="sxs-lookup"><span data-stu-id="715ee-109">Type</span></span>|<span data-ttu-id="715ee-110">説明</span><span class="sxs-lookup"><span data-stu-id="715ee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="715ee-111">profileId</span><span class="sxs-lookup"><span data-stu-id="715ee-111">profileId</span></span>|<span data-ttu-id="715ee-112">String</span><span class="sxs-lookup"><span data-stu-id="715ee-112">String</span></span>|<span data-ttu-id="715ee-113">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="715ee-113">Key of the entity.</span></span>|
|<span data-ttu-id="715ee-114">profileName</span><span class="sxs-lookup"><span data-stu-id="715ee-114">profileName</span></span>|<span data-ttu-id="715ee-115">String</span><span class="sxs-lookup"><span data-stu-id="715ee-115">String</span></span>|<span data-ttu-id="715ee-116">これは、アプリケーションのグループ、[スタート] メニューにこれらのアプリのレイアウト、およびこのキオスク構成を割り当てるユーザーを識別するために使用されるフレンドリ名です。</span><span class="sxs-lookup"><span data-stu-id="715ee-116">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="715ee-117">appconfiguration</span><span class="sxs-lookup"><span data-stu-id="715ee-117">appConfiguration</span></span>|[<span data-ttu-id="715ee-118">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="715ee-118">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="715ee-119">このキオスク構成で使用されるアプリ構成。</span><span class="sxs-lookup"><span data-stu-id="715ee-119">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="715ee-120">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="715ee-120">userAccountsConfiguration</span></span>|<span data-ttu-id="715ee-121">[windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="715ee-121">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="715ee-122">このキオスク構成にロックされるユーザーアカウント。</span><span class="sxs-lookup"><span data-stu-id="715ee-122">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="715ee-123">このコレクションには、最大100個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="715ee-123">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="715ee-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="715ee-124">Relationships</span></span>
<span data-ttu-id="715ee-125">なし</span><span class="sxs-lookup"><span data-stu-id="715ee-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="715ee-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="715ee-126">JSON Representation</span></span>
<span data-ttu-id="715ee-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="715ee-127">Here is a JSON representation of the resource.</span></span>
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
        "appUserModelId": "String",
        "appId": "String",
        "containedAppId": "String"
      }
    ],
    "showTaskBar": true,
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




