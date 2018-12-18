---
title: windowsPackageInformation リソースの種類
description: パッケージについては、ビジネス アプリケーションのウィンドウの行のプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: dcc277c610e6ceb27a94ab41993e599a258dd55e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342827"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="147a7-103">windowsPackageInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="147a7-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="147a7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="147a7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="147a7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="147a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="147a7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="147a7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="147a7-107">パッケージについては、ビジネス アプリケーションのウィンドウの行のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="147a7-107">Contains properties for the package information for a Windows line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="147a7-108">Properties</span><span class="sxs-lookup"><span data-stu-id="147a7-108">Properties</span></span>
|<span data-ttu-id="147a7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="147a7-109">Property</span></span>|<span data-ttu-id="147a7-110">種類</span><span class="sxs-lookup"><span data-stu-id="147a7-110">Type</span></span>|<span data-ttu-id="147a7-111">説明</span><span class="sxs-lookup"><span data-stu-id="147a7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="147a7-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="147a7-112">applicableArchitecture</span></span>|[<span data-ttu-id="147a7-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="147a7-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="147a7-114">Windows のアーキテクチャでこのアプリケーションが実行できます。</span><span class="sxs-lookup"><span data-stu-id="147a7-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="147a7-115">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="147a7-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="147a7-116">displayName</span><span class="sxs-lookup"><span data-stu-id="147a7-116">displayName</span></span>|<span data-ttu-id="147a7-117">String</span><span class="sxs-lookup"><span data-stu-id="147a7-117">String</span></span>|<span data-ttu-id="147a7-118">表示名。</span><span class="sxs-lookup"><span data-stu-id="147a7-118">The Display Name.</span></span>|
|<span data-ttu-id="147a7-119">identityName</span><span class="sxs-lookup"><span data-stu-id="147a7-119">identityName</span></span>|<span data-ttu-id="147a7-120">String</span><span class="sxs-lookup"><span data-stu-id="147a7-120">String</span></span>|<span data-ttu-id="147a7-121">ID 名。</span><span class="sxs-lookup"><span data-stu-id="147a7-121">The Identity Name.</span></span>|
|<span data-ttu-id="147a7-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="147a7-122">identityPublisher</span></span>|<span data-ttu-id="147a7-123">String</span><span class="sxs-lookup"><span data-stu-id="147a7-123">String</span></span>|<span data-ttu-id="147a7-124">識別情報の発行元です。</span><span class="sxs-lookup"><span data-stu-id="147a7-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="147a7-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="147a7-125">identityResourceIdentifier</span></span>|<span data-ttu-id="147a7-126">String</span><span class="sxs-lookup"><span data-stu-id="147a7-126">String</span></span>|<span data-ttu-id="147a7-127">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="147a7-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="147a7-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="147a7-128">identityVersion</span></span>|<span data-ttu-id="147a7-129">String</span><span class="sxs-lookup"><span data-stu-id="147a7-129">String</span></span>|<span data-ttu-id="147a7-130">アイデンティティのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="147a7-130">The Identity Version.</span></span>|
|<span data-ttu-id="147a7-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="147a7-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="147a7-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="147a7-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="147a7-133">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="147a7-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="147a7-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="147a7-134">Relationships</span></span>
<span data-ttu-id="147a7-135">なし</span><span class="sxs-lookup"><span data-stu-id="147a7-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="147a7-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="147a7-136">JSON Representation</span></span>
<span data-ttu-id="147a7-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="147a7-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsPackageInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPackageInformation",
  "applicableArchitecture": "String",
  "displayName": "String",
  "identityName": "String",
  "identityPublisher": "String",
  "identityResourceIdentifier": "String",
  "identityVersion": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  }
}
```





