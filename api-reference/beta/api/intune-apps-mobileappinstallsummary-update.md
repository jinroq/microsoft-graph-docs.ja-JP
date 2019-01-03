---
title: MobileAppInstallSummary を更新します。
description: MobileAppInstallSummary オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 94dc7fa5023d26de91b4d64efda27332dd51de63
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315639"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="3fd8f-103">MobileAppInstallSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="3fd8f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fd8f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fd8f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fd8f-107">[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-107">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3fd8f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3fd8f-108">Prerequisites</span></span>
<span data-ttu-id="3fd8f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fd8f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3fd8f-111">Permission type</span></span>|<span data-ttu-id="3fd8f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3fd8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fd8f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3fd8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3fd8f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fd8f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3fd8f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3fd8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fd8f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-116">Not supported.</span></span>|
|<span data-ttu-id="3fd8f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3fd8f-117">Application</span></span>|<span data-ttu-id="3fd8f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fd8f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3fd8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="3fd8f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3fd8f-120">Request headers</span></span>
|<span data-ttu-id="3fd8f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3fd8f-121">Header</span></span>|<span data-ttu-id="3fd8f-122">値</span><span class="sxs-lookup"><span data-stu-id="3fd8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fd8f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fd8f-123">Authorization</span></span>|<span data-ttu-id="3fd8f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fd8f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3fd8f-125">Accept</span></span>|<span data-ttu-id="3fd8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fd8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fd8f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3fd8f-127">Request body</span></span>
<span data-ttu-id="3fd8f-128">要求の本文に[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-128">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="3fd8f-129">[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-129">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="3fd8f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3fd8f-130">Property</span></span>|<span data-ttu-id="3fd8f-131">種類</span><span class="sxs-lookup"><span data-stu-id="3fd8f-131">Type</span></span>|<span data-ttu-id="3fd8f-132">説明</span><span class="sxs-lookup"><span data-stu-id="3fd8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fd8f-133">ID</span><span class="sxs-lookup"><span data-stu-id="3fd8f-133">id</span></span>|<span data-ttu-id="3fd8f-134">String</span><span class="sxs-lookup"><span data-stu-id="3fd8f-134">String</span></span>|<span data-ttu-id="3fd8f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-135">Key of the entity.</span></span>|
|<span data-ttu-id="3fd8f-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3fd8f-136">installedDeviceCount</span></span>|<span data-ttu-id="3fd8f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3fd8f-137">Int32</span></span>|<span data-ttu-id="3fd8f-138">このアプリケーションを正常にインストールするデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-138">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="3fd8f-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3fd8f-139">failedDeviceCount</span></span>|<span data-ttu-id="3fd8f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3fd8f-140">Int32</span></span>|<span data-ttu-id="3fd8f-141">このアプリケーションのインストールに失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-141">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="3fd8f-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3fd8f-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="3fd8f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3fd8f-143">Int32</span></span>|<span data-ttu-id="3fd8f-144">このアプリケーションには適用されていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-144">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="3fd8f-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3fd8f-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="3fd8f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3fd8f-146">Int32</span></span>|<span data-ttu-id="3fd8f-147">このアプリケーションをインストールしていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-147">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="3fd8f-148">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3fd8f-148">pendingInstallDeviceCount</span></span>|<span data-ttu-id="3fd8f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3fd8f-149">Int32</span></span>|<span data-ttu-id="3fd8f-150">このアプリケーションをインストールするのには通知しているデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-150">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="3fd8f-151">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="3fd8f-151">installedUserCount</span></span>|<span data-ttu-id="3fd8f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3fd8f-152">Int32</span></span>|<span data-ttu-id="3fd8f-153">このアプリケーションをインストールするのにはデバイスがすべて成功しているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-153">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="3fd8f-154">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="3fd8f-154">failedUserCount</span></span>|<span data-ttu-id="3fd8f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="3fd8f-155">Int32</span></span>|<span data-ttu-id="3fd8f-156">1 を持っているユーザー、またはこのアプリケーションのインストールに失敗した複数のデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-156">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="3fd8f-157">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="3fd8f-157">notApplicableUserCount</span></span>|<span data-ttu-id="3fd8f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3fd8f-158">Int32</span></span>|<span data-ttu-id="3fd8f-159">デバイスがなかったすべてこのアプリケーションに適用可能なユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-159">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="3fd8f-160">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="3fd8f-160">notInstalledUserCount</span></span>|<span data-ttu-id="3fd8f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="3fd8f-161">Int32</span></span>|<span data-ttu-id="3fd8f-162">このアプリケーションがインストールされていない 1 つ以上のデバイスを持っているユーザーの数です。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-162">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="3fd8f-163">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="3fd8f-163">pendingInstallUserCount</span></span>|<span data-ttu-id="3fd8f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3fd8f-164">Int32</span></span>|<span data-ttu-id="3fd8f-165">1 を持っているユーザー、またはこのアプリケーションをインストールし、0 のデバイス障害を通知している複数のデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-165">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="3fd8f-166">応答</span><span class="sxs-lookup"><span data-stu-id="3fd8f-166">Response</span></span>
<span data-ttu-id="3fd8f-167">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fd8f-168">例</span><span class="sxs-lookup"><span data-stu-id="3fd8f-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="3fd8f-169">要求</span><span class="sxs-lookup"><span data-stu-id="3fd8f-169">Request</span></span>
<span data-ttu-id="3fd8f-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 312

{
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

### <a name="response"></a><span data-ttu-id="3fd8f-171">応答</span><span class="sxs-lookup"><span data-stu-id="3fd8f-171">Response</span></span>
<span data-ttu-id="3fd8f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3fd8f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




