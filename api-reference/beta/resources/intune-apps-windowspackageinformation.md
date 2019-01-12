---
title: windowsPackageInformation リソースの種類
description: パッケージについては、ビジネス アプリケーションのウィンドウの行のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac0f9aad1cdba1eaaac12754fd4a4d0ad4a6db32
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926849"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="1e10f-103">windowsPackageInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e10f-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="1e10f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1e10f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e10f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e10f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e10f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e10f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e10f-107">パッケージについては、ビジネス アプリケーションのウィンドウの行のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1e10f-107">Contains properties for the package information for a Windows line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="1e10f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e10f-108">Properties</span></span>
|<span data-ttu-id="1e10f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e10f-109">Property</span></span>|<span data-ttu-id="1e10f-110">種類</span><span class="sxs-lookup"><span data-stu-id="1e10f-110">Type</span></span>|<span data-ttu-id="1e10f-111">説明</span><span class="sxs-lookup"><span data-stu-id="1e10f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e10f-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="1e10f-112">applicableArchitecture</span></span>|[<span data-ttu-id="1e10f-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="1e10f-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="1e10f-114">Windows のアーキテクチャでこのアプリケーションが実行できます。</span><span class="sxs-lookup"><span data-stu-id="1e10f-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="1e10f-115">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="1e10f-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="1e10f-116">displayName</span><span class="sxs-lookup"><span data-stu-id="1e10f-116">displayName</span></span>|<span data-ttu-id="1e10f-117">String</span><span class="sxs-lookup"><span data-stu-id="1e10f-117">String</span></span>|<span data-ttu-id="1e10f-118">表示名。</span><span class="sxs-lookup"><span data-stu-id="1e10f-118">The Display Name.</span></span>|
|<span data-ttu-id="1e10f-119">identityName</span><span class="sxs-lookup"><span data-stu-id="1e10f-119">identityName</span></span>|<span data-ttu-id="1e10f-120">String</span><span class="sxs-lookup"><span data-stu-id="1e10f-120">String</span></span>|<span data-ttu-id="1e10f-121">ID 名。</span><span class="sxs-lookup"><span data-stu-id="1e10f-121">The Identity Name.</span></span>|
|<span data-ttu-id="1e10f-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="1e10f-122">identityPublisher</span></span>|<span data-ttu-id="1e10f-123">String</span><span class="sxs-lookup"><span data-stu-id="1e10f-123">String</span></span>|<span data-ttu-id="1e10f-124">識別情報の発行元です。</span><span class="sxs-lookup"><span data-stu-id="1e10f-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="1e10f-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1e10f-125">identityResourceIdentifier</span></span>|<span data-ttu-id="1e10f-126">String</span><span class="sxs-lookup"><span data-stu-id="1e10f-126">String</span></span>|<span data-ttu-id="1e10f-127">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="1e10f-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="1e10f-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1e10f-128">identityVersion</span></span>|<span data-ttu-id="1e10f-129">String</span><span class="sxs-lookup"><span data-stu-id="1e10f-129">String</span></span>|<span data-ttu-id="1e10f-130">アイデンティティのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="1e10f-130">The Identity Version.</span></span>|
|<span data-ttu-id="1e10f-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1e10f-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1e10f-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1e10f-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="1e10f-133">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="1e10f-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e10f-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1e10f-134">Relationships</span></span>
<span data-ttu-id="1e10f-135">なし</span><span class="sxs-lookup"><span data-stu-id="1e10f-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1e10f-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e10f-136">JSON Representation</span></span>
<span data-ttu-id="1e10f-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1e10f-137">Here is a JSON representation of the resource.</span></span>
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





