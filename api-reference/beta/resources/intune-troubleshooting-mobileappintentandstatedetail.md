---
title: mobileAppIntentAndStateDetail リソースの種類
description: 特定のデバイスのモバイルアプリの意図とインストール状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 381fde8c3631c640691af346cccd3199d9018c50
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010204"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="c7c6d-103">mobileAppIntentAndStateDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7c6d-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="c7c6d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7c6d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7c6d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c7c6d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7c6d-106">特定のデバイスのモバイルアプリの意図とインストール状態。</span><span class="sxs-lookup"><span data-stu-id="c7c6d-106">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="c7c6d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7c6d-107">Properties</span></span>
|<span data-ttu-id="c7c6d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7c6d-108">Property</span></span>|<span data-ttu-id="c7c6d-109">型</span><span class="sxs-lookup"><span data-stu-id="c7c6d-109">Type</span></span>|<span data-ttu-id="c7c6d-110">説明</span><span class="sxs-lookup"><span data-stu-id="c7c6d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7c6d-111">applicationId</span><span class="sxs-lookup"><span data-stu-id="c7c6d-111">applicationId</span></span>|<span data-ttu-id="c7c6d-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c7c6d-112">String</span></span>|<span data-ttu-id="c7c6d-113">MobieApp 識別子。</span><span class="sxs-lookup"><span data-stu-id="c7c6d-113">MobieApp identifier.</span></span>|
|<span data-ttu-id="c7c6d-114">displayName</span><span class="sxs-lookup"><span data-stu-id="c7c6d-114">displayName</span></span>|<span data-ttu-id="c7c6d-115">String</span><span class="sxs-lookup"><span data-stu-id="c7c6d-115">String</span></span>|<span data-ttu-id="c7c6d-116">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="c7c6d-116">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="c7c6d-117">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="c7c6d-117">mobileAppIntent</span></span>|[<span data-ttu-id="c7c6d-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="c7c6d-118">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="c7c6d-119">モバイルアプリの目的。</span><span class="sxs-lookup"><span data-stu-id="c7c6d-119">Mobile App Intent.</span></span> <span data-ttu-id="c7c6d-120">可能な値は、`available`、`notAvailable`、`requiredInstall`、`requiredUninstall`、`requiredAndAvailableInstall`、`availableInstallWithoutEnrollment`、`exclude` です。</span><span class="sxs-lookup"><span data-stu-id="c7c6d-120">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="c7c6d-121">displayVersion</span><span class="sxs-lookup"><span data-stu-id="c7c6d-121">displayVersion</span></span>|<span data-ttu-id="c7c6d-122">String</span><span class="sxs-lookup"><span data-stu-id="c7c6d-122">String</span></span>|<span data-ttu-id="c7c6d-123">アプリケーションの人間の読み取り可能なバージョン</span><span class="sxs-lookup"><span data-stu-id="c7c6d-123">Human readable version of the application</span></span>|
|<span data-ttu-id="c7c6d-124">installState</span><span class="sxs-lookup"><span data-stu-id="c7c6d-124">installState</span></span>|[<span data-ttu-id="c7c6d-125">Resultappstate</span><span class="sxs-lookup"><span data-stu-id="c7c6d-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="c7c6d-126">アプリのインストール状態。</span><span class="sxs-lookup"><span data-stu-id="c7c6d-126">The install state of the app.</span></span> <span data-ttu-id="c7c6d-127">可能な値は、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable` です。</span><span class="sxs-lookup"><span data-stu-id="c7c6d-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="c7c6d-128">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="c7c6d-128">supportedDeviceTypes</span></span>|<span data-ttu-id="c7c6d-129">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c7c6d-129">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="c7c6d-130">アプリでサポートされているプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="c7c6d-130">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7c6d-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c7c6d-131">Relationships</span></span>
<span data-ttu-id="c7c6d-132">なし</span><span class="sxs-lookup"><span data-stu-id="c7c6d-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7c6d-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7c6d-133">JSON Representation</span></span>
<span data-ttu-id="c7c6d-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c7c6d-134">Here is a JSON representation of the resource.</span></span>
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





