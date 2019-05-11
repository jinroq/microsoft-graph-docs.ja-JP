---
title: windowsPackageInformation リソースの種類
description: Windows 基幹業務アプリのパッケージ情報のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2803779830d0e2bb88a0a91a96abfc101d15cb66
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949501"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="329e3-103">windowsPackageInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="329e3-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="329e3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="329e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="329e3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="329e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="329e3-106">Windows 基幹業務アプリのパッケージ情報のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="329e3-106">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="329e3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="329e3-107">Properties</span></span>
|<span data-ttu-id="329e3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="329e3-108">Property</span></span>|<span data-ttu-id="329e3-109">型</span><span class="sxs-lookup"><span data-stu-id="329e3-109">Type</span></span>|<span data-ttu-id="329e3-110">説明</span><span class="sxs-lookup"><span data-stu-id="329e3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="329e3-111">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="329e3-111">applicableArchitecture</span></span>|[<span data-ttu-id="329e3-112">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="329e3-112">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="329e3-113">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="329e3-113">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="329e3-114">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="329e3-114">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="329e3-115">displayName</span><span class="sxs-lookup"><span data-stu-id="329e3-115">displayName</span></span>|<span data-ttu-id="329e3-116">String</span><span class="sxs-lookup"><span data-stu-id="329e3-116">String</span></span>|<span data-ttu-id="329e3-117">表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="329e3-117">The Display Name.</span></span>|
|<span data-ttu-id="329e3-118">identityName</span><span class="sxs-lookup"><span data-stu-id="329e3-118">identityName</span></span>|<span data-ttu-id="329e3-119">String</span><span class="sxs-lookup"><span data-stu-id="329e3-119">String</span></span>|<span data-ttu-id="329e3-120">ID 名。</span><span class="sxs-lookup"><span data-stu-id="329e3-120">The Identity Name.</span></span>|
|<span data-ttu-id="329e3-121">識別子の入力</span><span class="sxs-lookup"><span data-stu-id="329e3-121">identityPublisher</span></span>|<span data-ttu-id="329e3-122">String</span><span class="sxs-lookup"><span data-stu-id="329e3-122">String</span></span>|<span data-ttu-id="329e3-123">Id 発行者。</span><span class="sxs-lookup"><span data-stu-id="329e3-123">The Identity Publisher.</span></span>|
|<span data-ttu-id="329e3-124">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="329e3-124">identityResourceIdentifier</span></span>|<span data-ttu-id="329e3-125">String</span><span class="sxs-lookup"><span data-stu-id="329e3-125">String</span></span>|<span data-ttu-id="329e3-126">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="329e3-126">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="329e3-127">identityVersion</span><span class="sxs-lookup"><span data-stu-id="329e3-127">identityVersion</span></span>|<span data-ttu-id="329e3-128">String</span><span class="sxs-lookup"><span data-stu-id="329e3-128">String</span></span>|<span data-ttu-id="329e3-129">Id のバージョン。</span><span class="sxs-lookup"><span data-stu-id="329e3-129">The Identity Version.</span></span>|
|<span data-ttu-id="329e3-130">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="329e3-130">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="329e3-131">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="329e3-131">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="329e3-132">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="329e3-132">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="329e3-133">関係</span><span class="sxs-lookup"><span data-stu-id="329e3-133">Relationships</span></span>
<span data-ttu-id="329e3-134">なし</span><span class="sxs-lookup"><span data-stu-id="329e3-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="329e3-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="329e3-135">JSON Representation</span></span>
<span data-ttu-id="329e3-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="329e3-136">Here is a JSON representation of the resource.</span></span>
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




