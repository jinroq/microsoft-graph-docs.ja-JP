---
title: windowsPackageInformation リソースの種類
description: パッケージについては、ビジネス アプリケーションのウィンドウの行のプロパティが含まれています。
ms.openlocfilehash: a7676320d5aa2eeab1140e6cc631c4061d2c5d14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070890"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="e2147-103">windowsPackageInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e2147-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="e2147-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e2147-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2147-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2147-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2147-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e2147-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2147-107">パッケージについては、ビジネス アプリケーションのウィンドウの行のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e2147-107">Contains properties for the package information for a Windows line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="e2147-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2147-108">Properties</span></span>
|<span data-ttu-id="e2147-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2147-109">Property</span></span>|<span data-ttu-id="e2147-110">型</span><span class="sxs-lookup"><span data-stu-id="e2147-110">Type</span></span>|<span data-ttu-id="e2147-111">説明</span><span class="sxs-lookup"><span data-stu-id="e2147-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2147-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="e2147-112">applicableArchitecture</span></span>|[<span data-ttu-id="e2147-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e2147-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e2147-114">Windows のアーキテクチャでこのアプリケーションが実行できます。</span><span class="sxs-lookup"><span data-stu-id="e2147-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="e2147-115">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="e2147-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="e2147-116">displayName</span><span class="sxs-lookup"><span data-stu-id="e2147-116">displayName</span></span>|<span data-ttu-id="e2147-117">String</span><span class="sxs-lookup"><span data-stu-id="e2147-117">String</span></span>|<span data-ttu-id="e2147-118">表示名。</span><span class="sxs-lookup"><span data-stu-id="e2147-118">The Display Name.</span></span>|
|<span data-ttu-id="e2147-119">identityName</span><span class="sxs-lookup"><span data-stu-id="e2147-119">identityName</span></span>|<span data-ttu-id="e2147-120">String</span><span class="sxs-lookup"><span data-stu-id="e2147-120">String</span></span>|<span data-ttu-id="e2147-121">ID 名。</span><span class="sxs-lookup"><span data-stu-id="e2147-121">The Identity Name.</span></span>|
|<span data-ttu-id="e2147-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="e2147-122">identityPublisher</span></span>|<span data-ttu-id="e2147-123">String</span><span class="sxs-lookup"><span data-stu-id="e2147-123">String</span></span>|<span data-ttu-id="e2147-124">識別情報の発行元です。</span><span class="sxs-lookup"><span data-stu-id="e2147-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="e2147-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e2147-125">identityResourceIdentifier</span></span>|<span data-ttu-id="e2147-126">String</span><span class="sxs-lookup"><span data-stu-id="e2147-126">String</span></span>|<span data-ttu-id="e2147-127">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="e2147-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="e2147-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e2147-128">identityVersion</span></span>|<span data-ttu-id="e2147-129">String</span><span class="sxs-lookup"><span data-stu-id="e2147-129">String</span></span>|<span data-ttu-id="e2147-130">アイデンティティのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="e2147-130">The Identity Version.</span></span>|
|<span data-ttu-id="e2147-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e2147-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e2147-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e2147-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="e2147-133">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="e2147-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2147-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e2147-134">Relationships</span></span>
<span data-ttu-id="e2147-135">なし</span><span class="sxs-lookup"><span data-stu-id="e2147-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2147-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2147-136">JSON Representation</span></span>
<span data-ttu-id="e2147-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e2147-137">Here is a JSON representation of the resource.</span></span>
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





