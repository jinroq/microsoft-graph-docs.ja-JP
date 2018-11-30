---
title: mobileAppInstallSummary リソースの種類
description: モバイル アプリケーションのインストールの概要のプロパティが含まれています。
ms.openlocfilehash: bda3f798a86b38ca0d1224ce509c355a8aec998a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066956"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="06a62-103">mobileAppInstallSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06a62-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="06a62-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="06a62-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06a62-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06a62-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06a62-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="06a62-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06a62-107">モバイル アプリケーションのインストールの概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="06a62-107">Contains properties for the installation summary of a mobile app.</span></span>
## <a name="methods"></a><span data-ttu-id="06a62-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="06a62-108">Methods</span></span>
|<span data-ttu-id="06a62-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="06a62-109">Method</span></span>|<span data-ttu-id="06a62-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="06a62-110">Return Type</span></span>|<span data-ttu-id="06a62-111">説明</span><span class="sxs-lookup"><span data-stu-id="06a62-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06a62-112">MobileAppInstallSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="06a62-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="06a62-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="06a62-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="06a62-114">[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06a62-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="06a62-115">MobileAppInstallSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="06a62-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="06a62-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="06a62-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="06a62-117">[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="06a62-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06a62-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06a62-118">Properties</span></span>
|<span data-ttu-id="06a62-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06a62-119">Property</span></span>|<span data-ttu-id="06a62-120">型</span><span class="sxs-lookup"><span data-stu-id="06a62-120">Type</span></span>|<span data-ttu-id="06a62-121">説明</span><span class="sxs-lookup"><span data-stu-id="06a62-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06a62-122">id</span><span class="sxs-lookup"><span data-stu-id="06a62-122">id</span></span>|<span data-ttu-id="06a62-123">String</span><span class="sxs-lookup"><span data-stu-id="06a62-123">String</span></span>|<span data-ttu-id="06a62-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="06a62-124">Key of the entity.</span></span>|
|<span data-ttu-id="06a62-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06a62-125">installedDeviceCount</span></span>|<span data-ttu-id="06a62-126">Int32</span><span class="sxs-lookup"><span data-stu-id="06a62-126">Int32</span></span>|<span data-ttu-id="06a62-127">このアプリケーションを正常にインストールするデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="06a62-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="06a62-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06a62-128">failedDeviceCount</span></span>|<span data-ttu-id="06a62-129">Int32</span><span class="sxs-lookup"><span data-stu-id="06a62-129">Int32</span></span>|<span data-ttu-id="06a62-130">このアプリケーションのインストールに失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="06a62-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="06a62-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06a62-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="06a62-132">Int32</span><span class="sxs-lookup"><span data-stu-id="06a62-132">Int32</span></span>|<span data-ttu-id="06a62-133">このアプリケーションには適用されていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="06a62-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="06a62-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06a62-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="06a62-135">Int32</span><span class="sxs-lookup"><span data-stu-id="06a62-135">Int32</span></span>|<span data-ttu-id="06a62-136">このアプリケーションをインストールしていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="06a62-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="06a62-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06a62-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="06a62-138">Int32</span><span class="sxs-lookup"><span data-stu-id="06a62-138">Int32</span></span>|<span data-ttu-id="06a62-139">このアプリケーションをインストールするのには通知しているデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="06a62-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="06a62-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="06a62-140">installedUserCount</span></span>|<span data-ttu-id="06a62-141">Int32</span><span class="sxs-lookup"><span data-stu-id="06a62-141">Int32</span></span>|<span data-ttu-id="06a62-142">このアプリケーションをインストールするのにはデバイスがすべて成功しているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="06a62-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="06a62-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="06a62-143">failedUserCount</span></span>|<span data-ttu-id="06a62-144">Int32</span><span class="sxs-lookup"><span data-stu-id="06a62-144">Int32</span></span>|<span data-ttu-id="06a62-145">1 を持っているユーザー、またはこのアプリケーションのインストールに失敗した複数のデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="06a62-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="06a62-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="06a62-146">notApplicableUserCount</span></span>|<span data-ttu-id="06a62-147">Int32</span><span class="sxs-lookup"><span data-stu-id="06a62-147">Int32</span></span>|<span data-ttu-id="06a62-148">デバイスがなかったすべてこのアプリケーションに適用可能なユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="06a62-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="06a62-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="06a62-149">notInstalledUserCount</span></span>|<span data-ttu-id="06a62-150">Int32</span><span class="sxs-lookup"><span data-stu-id="06a62-150">Int32</span></span>|<span data-ttu-id="06a62-151">このアプリケーションがインストールされていない 1 つ以上のデバイスを持っているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="06a62-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="06a62-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="06a62-152">pendingInstallUserCount</span></span>|<span data-ttu-id="06a62-153">Int32</span><span class="sxs-lookup"><span data-stu-id="06a62-153">Int32</span></span>|<span data-ttu-id="06a62-154">1 を持っているユーザー、またはこのアプリケーションをインストールし、0 のデバイス障害を通知している複数のデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="06a62-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06a62-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="06a62-155">Relationships</span></span>
<span data-ttu-id="06a62-156">なし</span><span class="sxs-lookup"><span data-stu-id="06a62-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="06a62-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06a62-157">JSON Representation</span></span>
<span data-ttu-id="06a62-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="06a62-158">Here is a JSON representation of the resource.</span></span>
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





