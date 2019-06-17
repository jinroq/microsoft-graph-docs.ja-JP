---
title: mobileAppInstallSummary リソースの種類
description: モバイルアプリのインストールの概要のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1e1d1a815ba1d4c688819a8d94c8acdd5beffca
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991829"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="2c201-103">mobileAppInstallSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c201-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="2c201-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c201-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c201-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2c201-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c201-106">モバイルアプリのインストールの概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2c201-106">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="2c201-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2c201-107">Methods</span></span>
|<span data-ttu-id="2c201-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2c201-108">Method</span></span>|<span data-ttu-id="2c201-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2c201-109">Return Type</span></span>|<span data-ttu-id="2c201-110">説明</span><span class="sxs-lookup"><span data-stu-id="2c201-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2c201-111">MobileAppInstallSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="2c201-111">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="2c201-112">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="2c201-112">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="2c201-113">[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2c201-113">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="2c201-114">MobileAppInstallSummary の更新</span><span class="sxs-lookup"><span data-stu-id="2c201-114">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="2c201-115">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="2c201-115">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="2c201-116">[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2c201-116">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c201-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c201-117">Properties</span></span>
|<span data-ttu-id="2c201-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c201-118">Property</span></span>|<span data-ttu-id="2c201-119">型</span><span class="sxs-lookup"><span data-stu-id="2c201-119">Type</span></span>|<span data-ttu-id="2c201-120">説明</span><span class="sxs-lookup"><span data-stu-id="2c201-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c201-121">id</span><span class="sxs-lookup"><span data-stu-id="2c201-121">id</span></span>|<span data-ttu-id="2c201-122">String</span><span class="sxs-lookup"><span data-stu-id="2c201-122">String</span></span>|<span data-ttu-id="2c201-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2c201-123">Key of the entity.</span></span>|
|<span data-ttu-id="2c201-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2c201-124">installedDeviceCount</span></span>|<span data-ttu-id="2c201-125">Int32</span><span class="sxs-lookup"><span data-stu-id="2c201-125">Int32</span></span>|<span data-ttu-id="2c201-126">このアプリが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="2c201-126">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="2c201-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2c201-127">failedDeviceCount</span></span>|<span data-ttu-id="2c201-128">Int32</span><span class="sxs-lookup"><span data-stu-id="2c201-128">Int32</span></span>|<span data-ttu-id="2c201-129">このアプリのインストールに失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="2c201-129">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="2c201-130">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2c201-130">notApplicableDeviceCount</span></span>|<span data-ttu-id="2c201-131">Int32</span><span class="sxs-lookup"><span data-stu-id="2c201-131">Int32</span></span>|<span data-ttu-id="2c201-132">このアプリに適用されないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="2c201-132">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="2c201-133">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2c201-133">notInstalledDeviceCount</span></span>|<span data-ttu-id="2c201-134">Int32</span><span class="sxs-lookup"><span data-stu-id="2c201-134">Int32</span></span>|<span data-ttu-id="2c201-135">このアプリがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="2c201-135">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="2c201-136">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2c201-136">pendingInstallDeviceCount</span></span>|<span data-ttu-id="2c201-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2c201-137">Int32</span></span>|<span data-ttu-id="2c201-138">このアプリをインストールするように通知されたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="2c201-138">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="2c201-139">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="2c201-139">installedUserCount</span></span>|<span data-ttu-id="2c201-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2c201-140">Int32</span></span>|<span data-ttu-id="2c201-141">このアプリをインストールするためにすべてのデバイスが正常に終了したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="2c201-141">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="2c201-142">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="2c201-142">failedUserCount</span></span>|<span data-ttu-id="2c201-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2c201-143">Int32</span></span>|<span data-ttu-id="2c201-144">このアプリのインストールに失敗した1つ以上のデバイスを持つユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="2c201-144">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="2c201-145">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="2c201-145">notApplicableUserCount</span></span>|<span data-ttu-id="2c201-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2c201-146">Int32</span></span>|<span data-ttu-id="2c201-147">このアプリに適用されていないデバイスを持つユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="2c201-147">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="2c201-148">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="2c201-148">notInstalledUserCount</span></span>|<span data-ttu-id="2c201-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2c201-149">Int32</span></span>|<span data-ttu-id="2c201-150">このアプリをインストールしなかった1つ以上のデバイスを持つユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="2c201-150">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="2c201-151">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="2c201-151">pendingInstallUserCount</span></span>|<span data-ttu-id="2c201-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2c201-152">Int32</span></span>|<span data-ttu-id="2c201-153">このアプリをインストールするように通知された1つ以上のデバイスを保有していて、エラーがあるデバイスが0個あるユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="2c201-153">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c201-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2c201-154">Relationships</span></span>
<span data-ttu-id="2c201-155">なし</span><span class="sxs-lookup"><span data-stu-id="2c201-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c201-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c201-156">JSON Representation</span></span>
<span data-ttu-id="2c201-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2c201-157">Here is a JSON representation of the resource.</span></span>
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





