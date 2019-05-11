---
title: MobileAppInstallSummary の更新
description: MobileAppInstallSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cff057bdb80e57fa2bdfcf4b9c008dacd0a58b42
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935090"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="4c60b-103">MobileAppInstallSummary の更新</span><span class="sxs-lookup"><span data-stu-id="4c60b-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="4c60b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c60b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c60b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c60b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c60b-106">[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4c60b-106">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c60b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4c60b-107">Prerequisites</span></span>
<span data-ttu-id="4c60b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c60b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c60b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c60b-110">Permission type</span></span>|<span data-ttu-id="4c60b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c60b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c60b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c60b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c60b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c60b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c60b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c60b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c60b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c60b-115">Not supported.</span></span>|
|<span data-ttu-id="4c60b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c60b-116">Application</span></span>|<span data-ttu-id="4c60b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c60b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c60b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c60b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="4c60b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c60b-119">Request headers</span></span>
|<span data-ttu-id="4c60b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c60b-120">Header</span></span>|<span data-ttu-id="4c60b-121">値</span><span class="sxs-lookup"><span data-stu-id="4c60b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c60b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c60b-122">Authorization</span></span>|<span data-ttu-id="4c60b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c60b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c60b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4c60b-124">Accept</span></span>|<span data-ttu-id="4c60b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c60b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c60b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c60b-126">Request body</span></span>
<span data-ttu-id="4c60b-127">要求本文で、 [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c60b-127">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="4c60b-128">次の表に、 [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4c60b-128">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="4c60b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c60b-129">Property</span></span>|<span data-ttu-id="4c60b-130">型</span><span class="sxs-lookup"><span data-stu-id="4c60b-130">Type</span></span>|<span data-ttu-id="4c60b-131">説明</span><span class="sxs-lookup"><span data-stu-id="4c60b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c60b-132">id</span><span class="sxs-lookup"><span data-stu-id="4c60b-132">id</span></span>|<span data-ttu-id="4c60b-133">String</span><span class="sxs-lookup"><span data-stu-id="4c60b-133">String</span></span>|<span data-ttu-id="4c60b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4c60b-134">Key of the entity.</span></span>|
|<span data-ttu-id="4c60b-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c60b-135">installedDeviceCount</span></span>|<span data-ttu-id="4c60b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4c60b-136">Int32</span></span>|<span data-ttu-id="4c60b-137">このアプリが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="4c60b-137">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="4c60b-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c60b-138">failedDeviceCount</span></span>|<span data-ttu-id="4c60b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4c60b-139">Int32</span></span>|<span data-ttu-id="4c60b-140">このアプリのインストールに失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="4c60b-140">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="4c60b-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c60b-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="4c60b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4c60b-142">Int32</span></span>|<span data-ttu-id="4c60b-143">このアプリに適用されないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="4c60b-143">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="4c60b-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c60b-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="4c60b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4c60b-145">Int32</span></span>|<span data-ttu-id="4c60b-146">このアプリがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="4c60b-146">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="4c60b-147">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c60b-147">pendingInstallDeviceCount</span></span>|<span data-ttu-id="4c60b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4c60b-148">Int32</span></span>|<span data-ttu-id="4c60b-149">このアプリをインストールするように通知されたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="4c60b-149">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="4c60b-150">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="4c60b-150">installedUserCount</span></span>|<span data-ttu-id="4c60b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="4c60b-151">Int32</span></span>|<span data-ttu-id="4c60b-152">このアプリをインストールするためにすべてのデバイスが正常に終了したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="4c60b-152">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="4c60b-153">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="4c60b-153">failedUserCount</span></span>|<span data-ttu-id="4c60b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="4c60b-154">Int32</span></span>|<span data-ttu-id="4c60b-155">このアプリのインストールに失敗した1つ以上のデバイスを持つユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="4c60b-155">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="4c60b-156">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="4c60b-156">notApplicableUserCount</span></span>|<span data-ttu-id="4c60b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4c60b-157">Int32</span></span>|<span data-ttu-id="4c60b-158">このアプリに適用されていないデバイスを持つユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="4c60b-158">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="4c60b-159">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="4c60b-159">notInstalledUserCount</span></span>|<span data-ttu-id="4c60b-160">Int32</span><span class="sxs-lookup"><span data-stu-id="4c60b-160">Int32</span></span>|<span data-ttu-id="4c60b-161">このアプリをインストールしなかった1つ以上のデバイスを持つユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="4c60b-161">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="4c60b-162">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="4c60b-162">pendingInstallUserCount</span></span>|<span data-ttu-id="4c60b-163">Int32</span><span class="sxs-lookup"><span data-stu-id="4c60b-163">Int32</span></span>|<span data-ttu-id="4c60b-164">このアプリをインストールするように通知された1つ以上のデバイスを保有していて、エラーがあるデバイスが0個あるユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="4c60b-164">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="4c60b-165">応答</span><span class="sxs-lookup"><span data-stu-id="4c60b-165">Response</span></span>
<span data-ttu-id="4c60b-166">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c60b-166">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c60b-167">例</span><span class="sxs-lookup"><span data-stu-id="4c60b-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c60b-168">要求</span><span class="sxs-lookup"><span data-stu-id="4c60b-168">Request</span></span>
<span data-ttu-id="4c60b-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4c60b-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4c60b-170">応答</span><span class="sxs-lookup"><span data-stu-id="4c60b-170">Response</span></span>
<span data-ttu-id="4c60b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c60b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




