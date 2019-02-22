---
title: mobileAppInstallSummary の更新
description: mobileAppInstallSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6065083d5ceb5892a95a6b12bc99657eca7d3eeb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152956"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="dcebe-103">mobileAppInstallSummary の更新</span><span class="sxs-lookup"><span data-stu-id="dcebe-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="dcebe-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcebe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcebe-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dcebe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcebe-106">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dcebe-106">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcebe-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="dcebe-107">Prerequisites</span></span>
<span data-ttu-id="dcebe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcebe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dcebe-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dcebe-110">Permission type</span></span>|<span data-ttu-id="dcebe-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dcebe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcebe-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dcebe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dcebe-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcebe-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dcebe-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dcebe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcebe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcebe-115">Not supported.</span></span>|
|<span data-ttu-id="dcebe-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dcebe-116">Application</span></span>|<span data-ttu-id="dcebe-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcebe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcebe-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dcebe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="dcebe-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dcebe-119">Request headers</span></span>
|<span data-ttu-id="dcebe-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dcebe-120">Header</span></span>|<span data-ttu-id="dcebe-121">値</span><span class="sxs-lookup"><span data-stu-id="dcebe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcebe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcebe-122">Authorization</span></span>|<span data-ttu-id="dcebe-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dcebe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcebe-124">承諾</span><span class="sxs-lookup"><span data-stu-id="dcebe-124">Accept</span></span>|<span data-ttu-id="dcebe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dcebe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcebe-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="dcebe-126">Request body</span></span>
<span data-ttu-id="dcebe-127">要求本文で、 [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dcebe-127">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="dcebe-128">次の表に、 [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dcebe-128">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="dcebe-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcebe-129">Property</span></span>|<span data-ttu-id="dcebe-130">型</span><span class="sxs-lookup"><span data-stu-id="dcebe-130">Type</span></span>|<span data-ttu-id="dcebe-131">説明</span><span class="sxs-lookup"><span data-stu-id="dcebe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcebe-132">id</span><span class="sxs-lookup"><span data-stu-id="dcebe-132">id</span></span>|<span data-ttu-id="dcebe-133">String</span><span class="sxs-lookup"><span data-stu-id="dcebe-133">String</span></span>|<span data-ttu-id="dcebe-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dcebe-134">Key of the entity.</span></span>|
|<span data-ttu-id="dcebe-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dcebe-135">installedDeviceCount</span></span>|<span data-ttu-id="dcebe-136">Int32</span><span class="sxs-lookup"><span data-stu-id="dcebe-136">Int32</span></span>|<span data-ttu-id="dcebe-137">このアプリが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="dcebe-137">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="dcebe-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dcebe-138">failedDeviceCount</span></span>|<span data-ttu-id="dcebe-139">Int32</span><span class="sxs-lookup"><span data-stu-id="dcebe-139">Int32</span></span>|<span data-ttu-id="dcebe-140">このアプリのインストールに失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="dcebe-140">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="dcebe-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dcebe-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="dcebe-142">Int32</span><span class="sxs-lookup"><span data-stu-id="dcebe-142">Int32</span></span>|<span data-ttu-id="dcebe-143">このアプリに適用されないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="dcebe-143">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="dcebe-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dcebe-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="dcebe-145">Int32</span><span class="sxs-lookup"><span data-stu-id="dcebe-145">Int32</span></span>|<span data-ttu-id="dcebe-146">このアプリがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="dcebe-146">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="dcebe-147">pendinginstalldevicecount</span><span class="sxs-lookup"><span data-stu-id="dcebe-147">pendingInstallDeviceCount</span></span>|<span data-ttu-id="dcebe-148">Int32</span><span class="sxs-lookup"><span data-stu-id="dcebe-148">Int32</span></span>|<span data-ttu-id="dcebe-149">このアプリをインストールするように通知されたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="dcebe-149">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="dcebe-150">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="dcebe-150">installedUserCount</span></span>|<span data-ttu-id="dcebe-151">Int32</span><span class="sxs-lookup"><span data-stu-id="dcebe-151">Int32</span></span>|<span data-ttu-id="dcebe-152">このアプリをインストールするためにすべてのデバイスが正常に終了したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="dcebe-152">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="dcebe-153">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="dcebe-153">failedUserCount</span></span>|<span data-ttu-id="dcebe-154">Int32</span><span class="sxs-lookup"><span data-stu-id="dcebe-154">Int32</span></span>|<span data-ttu-id="dcebe-155">このアプリのインストールに失敗した1つ以上のデバイスを持つユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="dcebe-155">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="dcebe-156">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="dcebe-156">notApplicableUserCount</span></span>|<span data-ttu-id="dcebe-157">Int32</span><span class="sxs-lookup"><span data-stu-id="dcebe-157">Int32</span></span>|<span data-ttu-id="dcebe-158">このアプリに適用されていないデバイスを持つユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="dcebe-158">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="dcebe-159">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="dcebe-159">notInstalledUserCount</span></span>|<span data-ttu-id="dcebe-160">Int32</span><span class="sxs-lookup"><span data-stu-id="dcebe-160">Int32</span></span>|<span data-ttu-id="dcebe-161">このアプリをインストールしなかった1つ以上のデバイスを持つユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="dcebe-161">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="dcebe-162">pendinginstallusercount</span><span class="sxs-lookup"><span data-stu-id="dcebe-162">pendingInstallUserCount</span></span>|<span data-ttu-id="dcebe-163">Int32</span><span class="sxs-lookup"><span data-stu-id="dcebe-163">Int32</span></span>|<span data-ttu-id="dcebe-164">このアプリをインストールするように通知された1つ以上のデバイスを保有していて、エラーがあるデバイスが0個あるユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="dcebe-164">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="dcebe-165">応答</span><span class="sxs-lookup"><span data-stu-id="dcebe-165">Response</span></span>
<span data-ttu-id="dcebe-166">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dcebe-166">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcebe-167">例</span><span class="sxs-lookup"><span data-stu-id="dcebe-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcebe-168">要求</span><span class="sxs-lookup"><span data-stu-id="dcebe-168">Request</span></span>
<span data-ttu-id="dcebe-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dcebe-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```

### <a name="response"></a><span data-ttu-id="dcebe-170">応答</span><span class="sxs-lookup"><span data-stu-id="dcebe-170">Response</span></span>
<span data-ttu-id="dcebe-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dcebe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "06a792e9-92e9-06a7-e992-a706e992a706",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```




