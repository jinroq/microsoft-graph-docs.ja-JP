---
title: mobileAppInstallSummary リソースの種類
description: モバイル アプリケーションのインストールの概要のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a75dba8303d254aff911cc66931d52abb8b76c07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916027"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="ba9ff-103">mobileAppInstallSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba9ff-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="ba9ff-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba9ff-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba9ff-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba9ff-107">モバイル アプリケーションのインストールの概要のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-107">Contains properties for the installation summary of a mobile app.</span></span>
## <a name="methods"></a><span data-ttu-id="ba9ff-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ba9ff-108">Methods</span></span>
|<span data-ttu-id="ba9ff-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ba9ff-109">Method</span></span>|<span data-ttu-id="ba9ff-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ba9ff-110">Return Type</span></span>|<span data-ttu-id="ba9ff-111">説明</span><span class="sxs-lookup"><span data-stu-id="ba9ff-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ba9ff-112">MobileAppInstallSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="ba9ff-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ba9ff-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="ba9ff-114">[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="ba9ff-115">MobileAppInstallSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="ba9ff-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ba9ff-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="ba9ff-117">[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba9ff-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba9ff-118">Properties</span></span>
|<span data-ttu-id="ba9ff-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba9ff-119">Property</span></span>|<span data-ttu-id="ba9ff-120">型</span><span class="sxs-lookup"><span data-stu-id="ba9ff-120">Type</span></span>|<span data-ttu-id="ba9ff-121">説明</span><span class="sxs-lookup"><span data-stu-id="ba9ff-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba9ff-122">ID</span><span class="sxs-lookup"><span data-stu-id="ba9ff-122">id</span></span>|<span data-ttu-id="ba9ff-123">String</span><span class="sxs-lookup"><span data-stu-id="ba9ff-123">String</span></span>|<span data-ttu-id="ba9ff-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-124">Key of the entity.</span></span>|
|<span data-ttu-id="ba9ff-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ba9ff-125">installedDeviceCount</span></span>|<span data-ttu-id="ba9ff-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9ff-126">Int32</span></span>|<span data-ttu-id="ba9ff-127">このアプリケーションを正常にインストールするデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="ba9ff-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ba9ff-128">failedDeviceCount</span></span>|<span data-ttu-id="ba9ff-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9ff-129">Int32</span></span>|<span data-ttu-id="ba9ff-130">このアプリケーションのインストールに失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="ba9ff-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ba9ff-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="ba9ff-132">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9ff-132">Int32</span></span>|<span data-ttu-id="ba9ff-133">このアプリケーションには適用されていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="ba9ff-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ba9ff-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="ba9ff-135">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9ff-135">Int32</span></span>|<span data-ttu-id="ba9ff-136">このアプリケーションをインストールしていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="ba9ff-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ba9ff-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="ba9ff-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9ff-138">Int32</span></span>|<span data-ttu-id="ba9ff-139">このアプリケーションをインストールするのには通知しているデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="ba9ff-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="ba9ff-140">installedUserCount</span></span>|<span data-ttu-id="ba9ff-141">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9ff-141">Int32</span></span>|<span data-ttu-id="ba9ff-142">このアプリケーションをインストールするのにはデバイスがすべて成功しているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="ba9ff-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="ba9ff-143">failedUserCount</span></span>|<span data-ttu-id="ba9ff-144">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9ff-144">Int32</span></span>|<span data-ttu-id="ba9ff-145">1 を持っているユーザー、またはこのアプリケーションのインストールに失敗した複数のデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="ba9ff-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="ba9ff-146">notApplicableUserCount</span></span>|<span data-ttu-id="ba9ff-147">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9ff-147">Int32</span></span>|<span data-ttu-id="ba9ff-148">デバイスがなかったすべてこのアプリケーションに適用可能なユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="ba9ff-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="ba9ff-149">notInstalledUserCount</span></span>|<span data-ttu-id="ba9ff-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9ff-150">Int32</span></span>|<span data-ttu-id="ba9ff-151">このアプリケーションがインストールされていない 1 つ以上のデバイスを持っているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="ba9ff-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="ba9ff-152">pendingInstallUserCount</span></span>|<span data-ttu-id="ba9ff-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9ff-153">Int32</span></span>|<span data-ttu-id="ba9ff-154">1 を持っているユーザー、またはこのアプリケーションをインストールし、0 のデバイス障害を通知している複数のデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba9ff-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ba9ff-155">Relationships</span></span>
<span data-ttu-id="ba9ff-156">なし</span><span class="sxs-lookup"><span data-stu-id="ba9ff-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ba9ff-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba9ff-157">JSON Representation</span></span>
<span data-ttu-id="ba9ff-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ba9ff-158">Here is a JSON representation of the resource.</span></span>
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





