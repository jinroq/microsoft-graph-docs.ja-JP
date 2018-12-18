---
title: deviceInstallState の更新
description: deviceInstallState オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 1f674b1c732b5804fd83c89620612354e8daccfa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325635"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="12c20-103">deviceInstallState の更新</span><span class="sxs-lookup"><span data-stu-id="12c20-103">Update deviceInstallState</span></span>

> <span data-ttu-id="12c20-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="12c20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12c20-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12c20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12c20-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="12c20-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12c20-107">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="12c20-107">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12c20-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="12c20-108">Prerequisites</span></span>
<span data-ttu-id="12c20-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12c20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12c20-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12c20-111">Permission type</span></span>|<span data-ttu-id="12c20-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="12c20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12c20-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12c20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12c20-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c20-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="12c20-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12c20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12c20-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12c20-116">Not supported.</span></span>|
|<span data-ttu-id="12c20-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12c20-117">Application</span></span>|<span data-ttu-id="12c20-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12c20-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12c20-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12c20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="12c20-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12c20-120">Request headers</span></span>
|<span data-ttu-id="12c20-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12c20-121">Header</span></span>|<span data-ttu-id="12c20-122">値</span><span class="sxs-lookup"><span data-stu-id="12c20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12c20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12c20-123">Authorization</span></span>|<span data-ttu-id="12c20-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="12c20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12c20-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12c20-125">Accept</span></span>|<span data-ttu-id="12c20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12c20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12c20-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="12c20-127">Request body</span></span>
<span data-ttu-id="12c20-128">要求本文で、[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="12c20-128">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="12c20-129">次の表に、[deviceInstallState](../resources/intune-books-deviceinstallstate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="12c20-129">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="12c20-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12c20-130">Property</span></span>|<span data-ttu-id="12c20-131">種類</span><span class="sxs-lookup"><span data-stu-id="12c20-131">Type</span></span>|<span data-ttu-id="12c20-132">説明</span><span class="sxs-lookup"><span data-stu-id="12c20-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12c20-133">ID</span><span class="sxs-lookup"><span data-stu-id="12c20-133">id</span></span>|<span data-ttu-id="12c20-134">String</span><span class="sxs-lookup"><span data-stu-id="12c20-134">String</span></span>|<span data-ttu-id="12c20-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="12c20-135">Key of the entity.</span></span>|
|<span data-ttu-id="12c20-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="12c20-136">deviceName</span></span>|<span data-ttu-id="12c20-137">String</span><span class="sxs-lookup"><span data-stu-id="12c20-137">String</span></span>|<span data-ttu-id="12c20-138">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="12c20-138">Device name.</span></span>|
|<span data-ttu-id="12c20-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="12c20-139">deviceId</span></span>|<span data-ttu-id="12c20-140">String</span><span class="sxs-lookup"><span data-stu-id="12c20-140">String</span></span>|<span data-ttu-id="12c20-141">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="12c20-141">Device Id.</span></span>|
|<span data-ttu-id="12c20-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="12c20-142">lastSyncDateTime</span></span>|<span data-ttu-id="12c20-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12c20-143">DateTimeOffset</span></span>|<span data-ttu-id="12c20-144">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="12c20-144">Last sync date and time.</span></span>|
|<span data-ttu-id="12c20-145">installState</span><span class="sxs-lookup"><span data-stu-id="12c20-145">installState</span></span>|[<span data-ttu-id="12c20-146">installState</span><span class="sxs-lookup"><span data-stu-id="12c20-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="12c20-147">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="12c20-147">The install state of the eBook.</span></span> <span data-ttu-id="12c20-148">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="12c20-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="12c20-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="12c20-149">errorCode</span></span>|<span data-ttu-id="12c20-150">String</span><span class="sxs-lookup"><span data-stu-id="12c20-150">String</span></span>|<span data-ttu-id="12c20-151">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="12c20-151">The error code for install failures.</span></span>|
|<span data-ttu-id="12c20-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="12c20-152">osVersion</span></span>|<span data-ttu-id="12c20-153">String</span><span class="sxs-lookup"><span data-stu-id="12c20-153">String</span></span>|<span data-ttu-id="12c20-154">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="12c20-154">OS Version.</span></span>|
|<span data-ttu-id="12c20-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="12c20-155">osDescription</span></span>|<span data-ttu-id="12c20-156">String</span><span class="sxs-lookup"><span data-stu-id="12c20-156">String</span></span>|<span data-ttu-id="12c20-157">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="12c20-157">OS Description.</span></span>|
|<span data-ttu-id="12c20-158">userName</span><span class="sxs-lookup"><span data-stu-id="12c20-158">userName</span></span>|<span data-ttu-id="12c20-159">String</span><span class="sxs-lookup"><span data-stu-id="12c20-159">String</span></span>|<span data-ttu-id="12c20-160">デバイスのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="12c20-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="12c20-161">応答</span><span class="sxs-lookup"><span data-stu-id="12c20-161">Response</span></span>
<span data-ttu-id="12c20-162">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="12c20-162">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12c20-163">例</span><span class="sxs-lookup"><span data-stu-id="12c20-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="12c20-164">要求</span><span class="sxs-lookup"><span data-stu-id="12c20-164">Request</span></span>
<span data-ttu-id="12c20-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="12c20-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
Content-type: application/json
Content-length: 317

{
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a><span data-ttu-id="12c20-166">応答</span><span class="sxs-lookup"><span data-stu-id="12c20-166">Response</span></span>
<span data-ttu-id="12c20-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="12c20-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```





