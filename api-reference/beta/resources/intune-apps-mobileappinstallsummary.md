---
title: mobileAppInstallSummary リソースの種類
description: モバイル アプリケーションのインストールの概要のプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2bd7c30c1b00e83731766bcd80f9a9fafd8e8b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416714"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="39f17-103">mobileAppInstallSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39f17-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="39f17-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="39f17-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="39f17-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39f17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39f17-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="39f17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39f17-107">モバイル アプリケーションのインストールの概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="39f17-107">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="39f17-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="39f17-108">Methods</span></span>
|<span data-ttu-id="39f17-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="39f17-109">Method</span></span>|<span data-ttu-id="39f17-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="39f17-110">Return Type</span></span>|<span data-ttu-id="39f17-111">説明</span><span class="sxs-lookup"><span data-stu-id="39f17-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39f17-112">MobileAppInstallSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="39f17-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="39f17-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="39f17-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="39f17-114">[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="39f17-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="39f17-115">MobileAppInstallSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="39f17-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="39f17-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="39f17-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="39f17-117">[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="39f17-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="39f17-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39f17-118">Properties</span></span>
|<span data-ttu-id="39f17-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39f17-119">Property</span></span>|<span data-ttu-id="39f17-120">型</span><span class="sxs-lookup"><span data-stu-id="39f17-120">Type</span></span>|<span data-ttu-id="39f17-121">説明</span><span class="sxs-lookup"><span data-stu-id="39f17-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39f17-122">id</span><span class="sxs-lookup"><span data-stu-id="39f17-122">id</span></span>|<span data-ttu-id="39f17-123">String</span><span class="sxs-lookup"><span data-stu-id="39f17-123">String</span></span>|<span data-ttu-id="39f17-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="39f17-124">Key of the entity.</span></span>|
|<span data-ttu-id="39f17-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39f17-125">installedDeviceCount</span></span>|<span data-ttu-id="39f17-126">Int32</span><span class="sxs-lookup"><span data-stu-id="39f17-126">Int32</span></span>|<span data-ttu-id="39f17-127">このアプリケーションを正常にインストールするデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="39f17-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="39f17-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39f17-128">failedDeviceCount</span></span>|<span data-ttu-id="39f17-129">Int32</span><span class="sxs-lookup"><span data-stu-id="39f17-129">Int32</span></span>|<span data-ttu-id="39f17-130">このアプリケーションのインストールに失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="39f17-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="39f17-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39f17-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="39f17-132">Int32</span><span class="sxs-lookup"><span data-stu-id="39f17-132">Int32</span></span>|<span data-ttu-id="39f17-133">このアプリケーションには適用されていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="39f17-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="39f17-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39f17-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="39f17-135">Int32</span><span class="sxs-lookup"><span data-stu-id="39f17-135">Int32</span></span>|<span data-ttu-id="39f17-136">このアプリケーションをインストールしていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="39f17-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="39f17-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="39f17-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="39f17-138">Int32</span><span class="sxs-lookup"><span data-stu-id="39f17-138">Int32</span></span>|<span data-ttu-id="39f17-139">このアプリケーションをインストールするのには通知しているデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="39f17-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="39f17-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="39f17-140">installedUserCount</span></span>|<span data-ttu-id="39f17-141">Int32</span><span class="sxs-lookup"><span data-stu-id="39f17-141">Int32</span></span>|<span data-ttu-id="39f17-142">このアプリケーションをインストールするのにはデバイスがすべて成功しているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="39f17-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="39f17-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="39f17-143">failedUserCount</span></span>|<span data-ttu-id="39f17-144">Int32</span><span class="sxs-lookup"><span data-stu-id="39f17-144">Int32</span></span>|<span data-ttu-id="39f17-145">1 を持っているユーザー、またはこのアプリケーションのインストールに失敗した複数のデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="39f17-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="39f17-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="39f17-146">notApplicableUserCount</span></span>|<span data-ttu-id="39f17-147">Int32</span><span class="sxs-lookup"><span data-stu-id="39f17-147">Int32</span></span>|<span data-ttu-id="39f17-148">デバイスがなかったすべてこのアプリケーションに適用可能なユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="39f17-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="39f17-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="39f17-149">notInstalledUserCount</span></span>|<span data-ttu-id="39f17-150">Int32</span><span class="sxs-lookup"><span data-stu-id="39f17-150">Int32</span></span>|<span data-ttu-id="39f17-151">このアプリケーションがインストールされていない 1 つ以上のデバイスを持っているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="39f17-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="39f17-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="39f17-152">pendingInstallUserCount</span></span>|<span data-ttu-id="39f17-153">Int32</span><span class="sxs-lookup"><span data-stu-id="39f17-153">Int32</span></span>|<span data-ttu-id="39f17-154">1 を持っているユーザー、またはこのアプリケーションをインストールし、0 のデバイス障害を通知している複数のデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="39f17-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39f17-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39f17-155">Relationships</span></span>
<span data-ttu-id="39f17-156">なし</span><span class="sxs-lookup"><span data-stu-id="39f17-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39f17-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39f17-157">JSON Representation</span></span>
<span data-ttu-id="39f17-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39f17-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "pendingInstallDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notApplicableUserCount": 1024,
  "notInstalledUserCount": 1024,
  "pendingInstallUserCount": 1024
}
```




