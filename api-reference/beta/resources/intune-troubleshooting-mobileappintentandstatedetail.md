---
title: mobileAppIntentAndStateDetail リソースの種類
description: モバイル アプリケーションの目的および特定のデバイスのインストールの状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 169988d8a3a114bbae7a06583565c9abd3414b4f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946687"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="e4072-103">mobileAppIntentAndStateDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e4072-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="e4072-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e4072-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4072-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4072-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4072-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4072-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4072-107">モバイル アプリケーションの目的および特定のデバイスのインストールの状態です。</span><span class="sxs-lookup"><span data-stu-id="e4072-107">Mobile App Intent and Install State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="e4072-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4072-108">Properties</span></span>
|<span data-ttu-id="e4072-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4072-109">Property</span></span>|<span data-ttu-id="e4072-110">種類</span><span class="sxs-lookup"><span data-stu-id="e4072-110">Type</span></span>|<span data-ttu-id="e4072-111">説明</span><span class="sxs-lookup"><span data-stu-id="e4072-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4072-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="e4072-112">applicationId</span></span>|<span data-ttu-id="e4072-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e4072-113">String</span></span>|<span data-ttu-id="e4072-114">MobieApp の識別子です。</span><span class="sxs-lookup"><span data-stu-id="e4072-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="e4072-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e4072-115">displayName</span></span>|<span data-ttu-id="e4072-116">String</span><span class="sxs-lookup"><span data-stu-id="e4072-116">String</span></span>|<span data-ttu-id="e4072-117">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="e4072-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="e4072-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="e4072-118">mobileAppIntent</span></span>|[<span data-ttu-id="e4072-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="e4072-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="e4072-120">モバイル アプリケーションの目的です。</span><span class="sxs-lookup"><span data-stu-id="e4072-120">Mobile App Intent.</span></span> <span data-ttu-id="e4072-121">可能な値は、`available`、`notAvailable`、`requiredInstall`、`requiredUninstall`、`requiredAndAvailableInstall`、`availableInstallWithoutEnrollment`、`exclude` です。</span><span class="sxs-lookup"><span data-stu-id="e4072-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="e4072-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="e4072-122">displayVersion</span></span>|<span data-ttu-id="e4072-123">String</span><span class="sxs-lookup"><span data-stu-id="e4072-123">String</span></span>|<span data-ttu-id="e4072-124">人間の読み取り可能なバージョンのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="e4072-124">Human readable version of the application</span></span>|
|<span data-ttu-id="e4072-125">installState</span><span class="sxs-lookup"><span data-stu-id="e4072-125">installState</span></span>|[<span data-ttu-id="e4072-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e4072-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e4072-127">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="e4072-127">The install state of the app.</span></span> <span data-ttu-id="e4072-128">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="e4072-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e4072-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="e4072-129">supportedDeviceTypes</span></span>|<span data-ttu-id="e4072-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e4072-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="e4072-131">アプリケーションのサポートされているプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="e4072-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4072-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e4072-132">Relationships</span></span>
<span data-ttu-id="e4072-133">なし</span><span class="sxs-lookup"><span data-stu-id="e4072-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e4072-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e4072-134">JSON Representation</span></span>
<span data-ttu-id="e4072-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e4072-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndStateDetail",
  "applicationId": "String",
  "displayName": "String",
  "mobileAppIntent": "String",
  "displayVersion": "String",
  "installState": "String",
  "supportedDeviceTypes": [
    {
      "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
      "type": "String",
      "minimumOperatingSystemVersion": "String",
      "maximumOperatingSystemVersion": "String"
    }
  ]
}
```





