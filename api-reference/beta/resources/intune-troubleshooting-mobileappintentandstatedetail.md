---
title: mobileAppIntentAndStateDetail リソースの種類
description: 特定のデバイスのモバイルアプリの意図とインストール状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e39a8e869a688dc74ebcc18e4ef56fc16459013d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777978"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="4c58e-103">mobileAppIntentAndStateDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c58e-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="4c58e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c58e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c58e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c58e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c58e-106">特定のデバイスのモバイルアプリの意図とインストール状態。</span><span class="sxs-lookup"><span data-stu-id="4c58e-106">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="4c58e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c58e-107">Properties</span></span>
|<span data-ttu-id="4c58e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c58e-108">Property</span></span>|<span data-ttu-id="4c58e-109">型</span><span class="sxs-lookup"><span data-stu-id="4c58e-109">Type</span></span>|<span data-ttu-id="4c58e-110">説明</span><span class="sxs-lookup"><span data-stu-id="4c58e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c58e-111">applicationId</span><span class="sxs-lookup"><span data-stu-id="4c58e-111">applicationId</span></span>|<span data-ttu-id="4c58e-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4c58e-112">String</span></span>|<span data-ttu-id="4c58e-113">MobieApp 識別子。</span><span class="sxs-lookup"><span data-stu-id="4c58e-113">MobieApp identifier.</span></span>|
|<span data-ttu-id="4c58e-114">displayName</span><span class="sxs-lookup"><span data-stu-id="4c58e-114">displayName</span></span>|<span data-ttu-id="4c58e-115">String</span><span class="sxs-lookup"><span data-stu-id="4c58e-115">String</span></span>|<span data-ttu-id="4c58e-116">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="4c58e-116">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="4c58e-117">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="4c58e-117">mobileAppIntent</span></span>|[<span data-ttu-id="4c58e-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="4c58e-118">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="4c58e-119">モバイルアプリの目的。</span><span class="sxs-lookup"><span data-stu-id="4c58e-119">Mobile App Intent.</span></span> <span data-ttu-id="4c58e-120">可能な値は、`available`、`notAvailable`、`requiredInstall`、`requiredUninstall`、`requiredAndAvailableInstall`、`availableInstallWithoutEnrollment`、`exclude` です。</span><span class="sxs-lookup"><span data-stu-id="4c58e-120">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="4c58e-121">displayversion</span><span class="sxs-lookup"><span data-stu-id="4c58e-121">displayVersion</span></span>|<span data-ttu-id="4c58e-122">文字列</span><span class="sxs-lookup"><span data-stu-id="4c58e-122">String</span></span>|<span data-ttu-id="4c58e-123">アプリケーションの人間の読み取り可能なバージョン</span><span class="sxs-lookup"><span data-stu-id="4c58e-123">Human readable version of the application</span></span>|
|<span data-ttu-id="4c58e-124">installState</span><span class="sxs-lookup"><span data-stu-id="4c58e-124">installState</span></span>|[<span data-ttu-id="4c58e-125">resultappstate</span><span class="sxs-lookup"><span data-stu-id="4c58e-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="4c58e-126">アプリのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="4c58e-126">The install state of the app.</span></span> <span data-ttu-id="4c58e-127">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="4c58e-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="4c58e-128">supporteddevicetypes</span><span class="sxs-lookup"><span data-stu-id="4c58e-128">supportedDeviceTypes</span></span>|<span data-ttu-id="4c58e-129">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4c58e-129">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="4c58e-130">アプリでサポートされているプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="4c58e-130">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c58e-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4c58e-131">Relationships</span></span>
<span data-ttu-id="4c58e-132">なし</span><span class="sxs-lookup"><span data-stu-id="4c58e-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c58e-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c58e-133">JSON Representation</span></span>
<span data-ttu-id="4c58e-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4c58e-134">Here is a JSON representation of the resource.</span></span>
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



