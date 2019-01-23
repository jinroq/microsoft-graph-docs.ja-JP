---
title: windowsKioskProfile リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55d8c23d3bfae2baf9d632c33390b8aafb5e7ef8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420249"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="37339-103">windowsKioskProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="37339-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="37339-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="37339-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37339-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37339-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37339-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="37339-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37339-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="37339-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="37339-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37339-108">Properties</span></span>
|<span data-ttu-id="37339-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37339-109">Property</span></span>|<span data-ttu-id="37339-110">型</span><span class="sxs-lookup"><span data-stu-id="37339-110">Type</span></span>|<span data-ttu-id="37339-111">説明</span><span class="sxs-lookup"><span data-stu-id="37339-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37339-112">プロファイル Id</span><span class="sxs-lookup"><span data-stu-id="37339-112">profileId</span></span>|<span data-ttu-id="37339-113">String</span><span class="sxs-lookup"><span data-stu-id="37339-113">String</span></span>|<span data-ttu-id="37339-114">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="37339-114">Key of the entity.</span></span>|
|<span data-ttu-id="37339-115">profilename プロパティ</span><span class="sxs-lookup"><span data-stu-id="37339-115">profileName</span></span>|<span data-ttu-id="37339-116">String</span><span class="sxs-lookup"><span data-stu-id="37339-116">String</span></span>|<span data-ttu-id="37339-117">これは、[スタート] メニューの [このプレゼンテーションの構成が割り当てられているユーザーにこれらのアプリケーションのレイアウト、アプリケーションのグループを識別するために使用するフレンドリ名です。</span><span class="sxs-lookup"><span data-stu-id="37339-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="37339-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="37339-118">appConfiguration</span></span>|[<span data-ttu-id="37339-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="37339-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="37339-120">このプレゼンテーションの構成を使用するアプリケーション構成します。</span><span class="sxs-lookup"><span data-stu-id="37339-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="37339-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="37339-121">userAccountsConfiguration</span></span>|<span data-ttu-id="37339-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="37339-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="37339-123">この構成にキオスクがロックアウトされているユーザー アカウントです。</span><span class="sxs-lookup"><span data-stu-id="37339-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="37339-124">このコレクションには、最大 100 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="37339-124">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37339-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="37339-125">Relationships</span></span>
<span data-ttu-id="37339-126">なし</span><span class="sxs-lookup"><span data-stu-id="37339-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37339-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="37339-127">JSON Representation</span></span>
<span data-ttu-id="37339-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="37339-128">Here is a JSON representation of the resource.</span></span>
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




