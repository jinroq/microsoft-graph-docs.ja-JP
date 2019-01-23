---
title: mobileAppIntentAndStateDetail リソースの種類
description: モバイル アプリケーションの目的および特定のデバイスのインストールの状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ef88a1fa346784ae00a125a487ca844c58d62eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414257"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="d3a3c-103">mobileAppIntentAndStateDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d3a3c-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="d3a3c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d3a3c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d3a3c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3a3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3a3c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3a3c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3a3c-107">モバイル アプリケーションの目的および特定のデバイスのインストールの状態です。</span><span class="sxs-lookup"><span data-stu-id="d3a3c-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="d3a3c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3a3c-108">Properties</span></span>
|<span data-ttu-id="d3a3c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3a3c-109">Property</span></span>|<span data-ttu-id="d3a3c-110">型</span><span class="sxs-lookup"><span data-stu-id="d3a3c-110">Type</span></span>|<span data-ttu-id="d3a3c-111">説明</span><span class="sxs-lookup"><span data-stu-id="d3a3c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3a3c-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="d3a3c-112">applicationId</span></span>|<span data-ttu-id="d3a3c-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d3a3c-113">String</span></span>|<span data-ttu-id="d3a3c-114">MobieApp の識別子です。</span><span class="sxs-lookup"><span data-stu-id="d3a3c-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="d3a3c-115">displayName</span><span class="sxs-lookup"><span data-stu-id="d3a3c-115">displayName</span></span>|<span data-ttu-id="d3a3c-116">String</span><span class="sxs-lookup"><span data-stu-id="d3a3c-116">String</span></span>|<span data-ttu-id="d3a3c-117">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="d3a3c-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="d3a3c-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="d3a3c-118">mobileAppIntent</span></span>|[<span data-ttu-id="d3a3c-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="d3a3c-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="d3a3c-120">モバイル アプリケーションの目的です。</span><span class="sxs-lookup"><span data-stu-id="d3a3c-120">Mobile App Intent.</span></span> <span data-ttu-id="d3a3c-121">可能な値は、`available`、`notAvailable`、`requiredInstall`、`requiredUninstall`、`requiredAndAvailableInstall`、`availableInstallWithoutEnrollment`、`exclude` です。</span><span class="sxs-lookup"><span data-stu-id="d3a3c-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="d3a3c-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="d3a3c-122">displayVersion</span></span>|<span data-ttu-id="d3a3c-123">String</span><span class="sxs-lookup"><span data-stu-id="d3a3c-123">String</span></span>|<span data-ttu-id="d3a3c-124">人間の読み取り可能なバージョンのアプリケーション</span><span class="sxs-lookup"><span data-stu-id="d3a3c-124">Human readable version of the application</span></span>|
|<span data-ttu-id="d3a3c-125">installState</span><span class="sxs-lookup"><span data-stu-id="d3a3c-125">installState</span></span>|[<span data-ttu-id="d3a3c-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="d3a3c-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="d3a3c-127">アプリケーションのインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="d3a3c-127">The install state of the app.</span></span> <span data-ttu-id="d3a3c-128">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="d3a3c-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="d3a3c-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="d3a3c-129">supportedDeviceTypes</span></span>|<span data-ttu-id="d3a3c-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d3a3c-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="d3a3c-131">アプリケーションのサポートされているプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="d3a3c-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3a3c-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d3a3c-132">Relationships</span></span>
<span data-ttu-id="d3a3c-133">なし</span><span class="sxs-lookup"><span data-stu-id="d3a3c-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3a3c-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d3a3c-134">JSON Representation</span></span>
<span data-ttu-id="d3a3c-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d3a3c-135">Here is a JSON representation of the resource.</span></span>
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




