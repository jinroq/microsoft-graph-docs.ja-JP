---
title: mobileAppInstallSummary リソースの種類
description: モバイル アプリケーションのインストールの概要のプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: d998e0fe5b136afe7aa18741c5c91fcde9adcc37
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314785"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="5a48e-103">mobileAppInstallSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a48e-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="5a48e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a48e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a48e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a48e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a48e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a48e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a48e-107">モバイル アプリケーションのインストールの概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a48e-107">Contains properties for the installation summary of a mobile app.</span></span>
## <a name="methods"></a><span data-ttu-id="5a48e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a48e-108">Methods</span></span>
|<span data-ttu-id="5a48e-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a48e-109">Method</span></span>|<span data-ttu-id="5a48e-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5a48e-110">Return Type</span></span>|<span data-ttu-id="5a48e-111">説明</span><span class="sxs-lookup"><span data-stu-id="5a48e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a48e-112">MobileAppInstallSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="5a48e-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="5a48e-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5a48e-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="5a48e-114">[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a48e-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="5a48e-115">MobileAppInstallSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="5a48e-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="5a48e-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5a48e-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="5a48e-117">[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5a48e-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5a48e-118">Properties</span><span class="sxs-lookup"><span data-stu-id="5a48e-118">Properties</span></span>
|<span data-ttu-id="5a48e-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a48e-119">Property</span></span>|<span data-ttu-id="5a48e-120">種類</span><span class="sxs-lookup"><span data-stu-id="5a48e-120">Type</span></span>|<span data-ttu-id="5a48e-121">説明</span><span class="sxs-lookup"><span data-stu-id="5a48e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a48e-122">ID</span><span class="sxs-lookup"><span data-stu-id="5a48e-122">id</span></span>|<span data-ttu-id="5a48e-123">String</span><span class="sxs-lookup"><span data-stu-id="5a48e-123">String</span></span>|<span data-ttu-id="5a48e-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5a48e-124">Key of the entity.</span></span>|
|<span data-ttu-id="5a48e-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a48e-125">installedDeviceCount</span></span>|<span data-ttu-id="5a48e-126">Int32</span><span class="sxs-lookup"><span data-stu-id="5a48e-126">Int32</span></span>|<span data-ttu-id="5a48e-127">このアプリケーションを正常にインストールするデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5a48e-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="5a48e-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a48e-128">failedDeviceCount</span></span>|<span data-ttu-id="5a48e-129">Int32</span><span class="sxs-lookup"><span data-stu-id="5a48e-129">Int32</span></span>|<span data-ttu-id="5a48e-130">このアプリケーションのインストールに失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="5a48e-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="5a48e-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a48e-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="5a48e-132">Int32</span><span class="sxs-lookup"><span data-stu-id="5a48e-132">Int32</span></span>|<span data-ttu-id="5a48e-133">このアプリケーションには適用されていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5a48e-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="5a48e-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a48e-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="5a48e-135">Int32</span><span class="sxs-lookup"><span data-stu-id="5a48e-135">Int32</span></span>|<span data-ttu-id="5a48e-136">このアプリケーションをインストールしていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="5a48e-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="5a48e-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a48e-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="5a48e-138">Int32</span><span class="sxs-lookup"><span data-stu-id="5a48e-138">Int32</span></span>|<span data-ttu-id="5a48e-139">このアプリケーションをインストールするのには通知しているデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5a48e-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="5a48e-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="5a48e-140">installedUserCount</span></span>|<span data-ttu-id="5a48e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5a48e-141">Int32</span></span>|<span data-ttu-id="5a48e-142">このアプリケーションをインストールするのにはデバイスがすべて成功しているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="5a48e-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="5a48e-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="5a48e-143">failedUserCount</span></span>|<span data-ttu-id="5a48e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="5a48e-144">Int32</span></span>|<span data-ttu-id="5a48e-145">1 を持っているユーザー、またはこのアプリケーションのインストールに失敗した複数のデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5a48e-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="5a48e-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="5a48e-146">notApplicableUserCount</span></span>|<span data-ttu-id="5a48e-147">Int32</span><span class="sxs-lookup"><span data-stu-id="5a48e-147">Int32</span></span>|<span data-ttu-id="5a48e-148">デバイスがなかったすべてこのアプリケーションに適用可能なユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="5a48e-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="5a48e-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="5a48e-149">notInstalledUserCount</span></span>|<span data-ttu-id="5a48e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5a48e-150">Int32</span></span>|<span data-ttu-id="5a48e-151">このアプリケーションがインストールされていない 1 つ以上のデバイスを持っているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="5a48e-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="5a48e-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="5a48e-152">pendingInstallUserCount</span></span>|<span data-ttu-id="5a48e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5a48e-153">Int32</span></span>|<span data-ttu-id="5a48e-154">1 を持っているユーザー、またはこのアプリケーションをインストールし、0 のデバイス障害を通知している複数のデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5a48e-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a48e-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a48e-155">Relationships</span></span>
<span data-ttu-id="5a48e-156">なし</span><span class="sxs-lookup"><span data-stu-id="5a48e-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5a48e-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a48e-157">JSON Representation</span></span>
<span data-ttu-id="5a48e-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a48e-158">Here is a JSON representation of the resource.</span></span>
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





