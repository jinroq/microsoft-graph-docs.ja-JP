---
title: windowspackageinformation リソースの種類
description: Windows 基幹業務アプリのパッケージ情報のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e1dda51d5c98cb27ab9e71c7bef9167959c9052
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799616"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="9f2cb-103">windowspackageinformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f2cb-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="9f2cb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f2cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f2cb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9f2cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f2cb-106">Windows 基幹業務アプリのパッケージ情報のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9f2cb-106">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="9f2cb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f2cb-107">Properties</span></span>
|<span data-ttu-id="9f2cb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f2cb-108">Property</span></span>|<span data-ttu-id="9f2cb-109">型</span><span class="sxs-lookup"><span data-stu-id="9f2cb-109">Type</span></span>|<span data-ttu-id="9f2cb-110">説明</span><span class="sxs-lookup"><span data-stu-id="9f2cb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f2cb-111">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="9f2cb-111">applicableArchitecture</span></span>|[<span data-ttu-id="9f2cb-112">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="9f2cb-112">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="9f2cb-113">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="9f2cb-113">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="9f2cb-114">可能な値は `none`、`x86`、`x64`、`arm`、`neutral`、`arm64` です。</span><span class="sxs-lookup"><span data-stu-id="9f2cb-114">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="9f2cb-115">displayName</span><span class="sxs-lookup"><span data-stu-id="9f2cb-115">displayName</span></span>|<span data-ttu-id="9f2cb-116">String</span><span class="sxs-lookup"><span data-stu-id="9f2cb-116">String</span></span>|<span data-ttu-id="9f2cb-117">表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="9f2cb-117">The Display Name.</span></span>|
|<span data-ttu-id="9f2cb-118">identityName</span><span class="sxs-lookup"><span data-stu-id="9f2cb-118">identityName</span></span>|<span data-ttu-id="9f2cb-119">文字列</span><span class="sxs-lookup"><span data-stu-id="9f2cb-119">String</span></span>|<span data-ttu-id="9f2cb-120">ID 名。</span><span class="sxs-lookup"><span data-stu-id="9f2cb-120">The Identity Name.</span></span>|
|<span data-ttu-id="9f2cb-121">識別子の入力</span><span class="sxs-lookup"><span data-stu-id="9f2cb-121">identityPublisher</span></span>|<span data-ttu-id="9f2cb-122">文字列</span><span class="sxs-lookup"><span data-stu-id="9f2cb-122">String</span></span>|<span data-ttu-id="9f2cb-123">id 発行者。</span><span class="sxs-lookup"><span data-stu-id="9f2cb-123">The Identity Publisher.</span></span>|
|<span data-ttu-id="9f2cb-124">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9f2cb-124">identityResourceIdentifier</span></span>|<span data-ttu-id="9f2cb-125">String</span><span class="sxs-lookup"><span data-stu-id="9f2cb-125">String</span></span>|<span data-ttu-id="9f2cb-126">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="9f2cb-126">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="9f2cb-127">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9f2cb-127">identityVersion</span></span>|<span data-ttu-id="9f2cb-128">String</span><span class="sxs-lookup"><span data-stu-id="9f2cb-128">String</span></span>|<span data-ttu-id="9f2cb-129">id のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9f2cb-129">The Identity Version.</span></span>|
|<span data-ttu-id="9f2cb-130">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9f2cb-130">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9f2cb-131">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9f2cb-131">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="9f2cb-132">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="9f2cb-132">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f2cb-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f2cb-133">Relationships</span></span>
<span data-ttu-id="9f2cb-134">なし</span><span class="sxs-lookup"><span data-stu-id="9f2cb-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f2cb-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f2cb-135">JSON Representation</span></span>
<span data-ttu-id="9f2cb-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f2cb-136">Here is a JSON representation of the resource.</span></span>
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





