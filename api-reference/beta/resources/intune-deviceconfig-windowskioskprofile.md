---
title: windowsKioskProfile リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: ce57b18e86f40a46053a5e0a0f41652763a6d055
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345354"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="29ed8-103">windowsKioskProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29ed8-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="29ed8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="29ed8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29ed8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29ed8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29ed8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="29ed8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29ed8-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29ed8-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="29ed8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29ed8-108">Properties</span></span>
|<span data-ttu-id="29ed8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29ed8-109">Property</span></span>|<span data-ttu-id="29ed8-110">種類</span><span class="sxs-lookup"><span data-stu-id="29ed8-110">Type</span></span>|<span data-ttu-id="29ed8-111">説明</span><span class="sxs-lookup"><span data-stu-id="29ed8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29ed8-112">プロファイル Id</span><span class="sxs-lookup"><span data-stu-id="29ed8-112">profileId</span></span>|<span data-ttu-id="29ed8-113">String</span><span class="sxs-lookup"><span data-stu-id="29ed8-113">String</span></span>|<span data-ttu-id="29ed8-114">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="29ed8-114">Key of the entity.</span></span>|
|<span data-ttu-id="29ed8-115">profilename プロパティ</span><span class="sxs-lookup"><span data-stu-id="29ed8-115">profileName</span></span>|<span data-ttu-id="29ed8-116">String</span><span class="sxs-lookup"><span data-stu-id="29ed8-116">String</span></span>|<span data-ttu-id="29ed8-117">これは、[スタート] メニューの [このプレゼンテーションの構成が割り当てられているユーザーにこれらのアプリケーションのレイアウト、アプリケーションのグループを識別するために使用するフレンドリ名です。</span><span class="sxs-lookup"><span data-stu-id="29ed8-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="29ed8-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="29ed8-118">appConfiguration</span></span>|[<span data-ttu-id="29ed8-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="29ed8-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="29ed8-120">このプレゼンテーションの構成を使用するアプリケーション構成します。</span><span class="sxs-lookup"><span data-stu-id="29ed8-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="29ed8-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="29ed8-121">userAccountsConfiguration</span></span>|<span data-ttu-id="29ed8-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="29ed8-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="29ed8-123">この構成にキオスクがロックアウトされているユーザー アカウントです。</span><span class="sxs-lookup"><span data-stu-id="29ed8-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="29ed8-124">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="29ed8-124">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29ed8-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29ed8-125">Relationships</span></span>
<span data-ttu-id="29ed8-126">なし</span><span class="sxs-lookup"><span data-stu-id="29ed8-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="29ed8-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29ed8-127">JSON Representation</span></span>
<span data-ttu-id="29ed8-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29ed8-128">Here is a JSON representation of the resource.</span></span>
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





