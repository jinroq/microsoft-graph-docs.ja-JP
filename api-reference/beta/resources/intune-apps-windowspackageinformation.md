---
title: windowsPackageInformation リソースの種類
description: パッケージについては、ビジネス アプリケーションのウィンドウの行のプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 112d84c5bae889e24b889b4598d61a6b3d63db50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403281"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="a0036-103">windowsPackageInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a0036-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="a0036-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a0036-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a0036-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0036-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0036-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a0036-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0036-107">パッケージについては、ビジネス アプリケーションのウィンドウの行のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a0036-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="a0036-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0036-108">Properties</span></span>
|<span data-ttu-id="a0036-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0036-109">Property</span></span>|<span data-ttu-id="a0036-110">型</span><span class="sxs-lookup"><span data-stu-id="a0036-110">Type</span></span>|<span data-ttu-id="a0036-111">説明</span><span class="sxs-lookup"><span data-stu-id="a0036-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0036-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="a0036-112">applicableArchitecture</span></span>|[<span data-ttu-id="a0036-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="a0036-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="a0036-114">Windows のアーキテクチャでこのアプリケーションが実行できます。</span><span class="sxs-lookup"><span data-stu-id="a0036-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="a0036-115">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="a0036-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="a0036-116">displayName</span><span class="sxs-lookup"><span data-stu-id="a0036-116">displayName</span></span>|<span data-ttu-id="a0036-117">String</span><span class="sxs-lookup"><span data-stu-id="a0036-117">String</span></span>|<span data-ttu-id="a0036-118">表示名。</span><span class="sxs-lookup"><span data-stu-id="a0036-118">The Display Name.</span></span>|
|<span data-ttu-id="a0036-119">identityName</span><span class="sxs-lookup"><span data-stu-id="a0036-119">identityName</span></span>|<span data-ttu-id="a0036-120">String</span><span class="sxs-lookup"><span data-stu-id="a0036-120">String</span></span>|<span data-ttu-id="a0036-121">ID 名。</span><span class="sxs-lookup"><span data-stu-id="a0036-121">The Identity Name.</span></span>|
|<span data-ttu-id="a0036-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="a0036-122">identityPublisher</span></span>|<span data-ttu-id="a0036-123">String</span><span class="sxs-lookup"><span data-stu-id="a0036-123">String</span></span>|<span data-ttu-id="a0036-124">識別情報の発行元です。</span><span class="sxs-lookup"><span data-stu-id="a0036-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="a0036-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a0036-125">identityResourceIdentifier</span></span>|<span data-ttu-id="a0036-126">String</span><span class="sxs-lookup"><span data-stu-id="a0036-126">String</span></span>|<span data-ttu-id="a0036-127">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="a0036-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="a0036-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="a0036-128">identityVersion</span></span>|<span data-ttu-id="a0036-129">String</span><span class="sxs-lookup"><span data-stu-id="a0036-129">String</span></span>|<span data-ttu-id="a0036-130">アイデンティティのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="a0036-130">The Identity Version.</span></span>|
|<span data-ttu-id="a0036-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a0036-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a0036-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a0036-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="a0036-133">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="a0036-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0036-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a0036-134">Relationships</span></span>
<span data-ttu-id="a0036-135">なし</span><span class="sxs-lookup"><span data-stu-id="a0036-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0036-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a0036-136">JSON Representation</span></span>
<span data-ttu-id="a0036-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a0036-137">Here is a JSON representation of the resource.</span></span>
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




