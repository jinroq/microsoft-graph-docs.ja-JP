---
title: deviceInstallState の更新
description: deviceInstallState オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 680cf388fdf2a09cbb9e553efad4dafc2b767e82
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36336083"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="2f788-103">deviceInstallState の更新</span><span class="sxs-lookup"><span data-stu-id="2f788-103">Update deviceInstallState</span></span>

> <span data-ttu-id="2f788-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f788-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f788-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2f788-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f788-106">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2f788-106">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f788-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2f788-107">Prerequisites</span></span>
<span data-ttu-id="2f788-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f788-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2f788-110">Permission type</span></span>|<span data-ttu-id="2f788-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2f788-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f788-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2f788-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f788-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f788-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2f788-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2f788-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f788-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f788-115">Not supported.</span></span>|
|<span data-ttu-id="2f788-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2f788-116">Application</span></span>|<span data-ttu-id="2f788-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f788-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f788-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2f788-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="2f788-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f788-119">Request headers</span></span>
|<span data-ttu-id="2f788-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f788-120">Header</span></span>|<span data-ttu-id="2f788-121">値</span><span class="sxs-lookup"><span data-stu-id="2f788-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f788-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f788-122">Authorization</span></span>|<span data-ttu-id="2f788-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2f788-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f788-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2f788-124">Accept</span></span>|<span data-ttu-id="2f788-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f788-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f788-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2f788-126">Request body</span></span>
<span data-ttu-id="2f788-127">要求本文で、[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2f788-127">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="2f788-128">次の表に、[deviceInstallState](../resources/intune-books-deviceinstallstate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2f788-128">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="2f788-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f788-129">Property</span></span>|<span data-ttu-id="2f788-130">型</span><span class="sxs-lookup"><span data-stu-id="2f788-130">Type</span></span>|<span data-ttu-id="2f788-131">説明</span><span class="sxs-lookup"><span data-stu-id="2f788-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f788-132">id</span><span class="sxs-lookup"><span data-stu-id="2f788-132">id</span></span>|<span data-ttu-id="2f788-133">String</span><span class="sxs-lookup"><span data-stu-id="2f788-133">String</span></span>|<span data-ttu-id="2f788-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2f788-134">Key of the entity.</span></span>|
|<span data-ttu-id="2f788-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="2f788-135">deviceName</span></span>|<span data-ttu-id="2f788-136">String</span><span class="sxs-lookup"><span data-stu-id="2f788-136">String</span></span>|<span data-ttu-id="2f788-137">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="2f788-137">Device name.</span></span>|
|<span data-ttu-id="2f788-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="2f788-138">deviceId</span></span>|<span data-ttu-id="2f788-139">String</span><span class="sxs-lookup"><span data-stu-id="2f788-139">String</span></span>|<span data-ttu-id="2f788-140">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="2f788-140">Device Id.</span></span>|
|<span data-ttu-id="2f788-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2f788-141">lastSyncDateTime</span></span>|<span data-ttu-id="2f788-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f788-142">DateTimeOffset</span></span>|<span data-ttu-id="2f788-143">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="2f788-143">Last sync date and time.</span></span>|
|<span data-ttu-id="2f788-144">installState</span><span class="sxs-lookup"><span data-stu-id="2f788-144">installState</span></span>|[<span data-ttu-id="2f788-145">installState</span><span class="sxs-lookup"><span data-stu-id="2f788-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="2f788-146">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="2f788-146">The install state of the eBook.</span></span> <span data-ttu-id="2f788-147">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="2f788-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="2f788-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="2f788-148">errorCode</span></span>|<span data-ttu-id="2f788-149">String</span><span class="sxs-lookup"><span data-stu-id="2f788-149">String</span></span>|<span data-ttu-id="2f788-150">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="2f788-150">The error code for install failures.</span></span>|
|<span data-ttu-id="2f788-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="2f788-151">osVersion</span></span>|<span data-ttu-id="2f788-152">String</span><span class="sxs-lookup"><span data-stu-id="2f788-152">String</span></span>|<span data-ttu-id="2f788-153">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="2f788-153">OS Version.</span></span>|
|<span data-ttu-id="2f788-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="2f788-154">osDescription</span></span>|<span data-ttu-id="2f788-155">String</span><span class="sxs-lookup"><span data-stu-id="2f788-155">String</span></span>|<span data-ttu-id="2f788-156">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="2f788-156">OS Description.</span></span>|
|<span data-ttu-id="2f788-157">userName</span><span class="sxs-lookup"><span data-stu-id="2f788-157">userName</span></span>|<span data-ttu-id="2f788-158">String</span><span class="sxs-lookup"><span data-stu-id="2f788-158">String</span></span>|<span data-ttu-id="2f788-159">デバイスのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="2f788-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="2f788-160">応答</span><span class="sxs-lookup"><span data-stu-id="2f788-160">Response</span></span>
<span data-ttu-id="2f788-161">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2f788-161">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f788-162">例</span><span class="sxs-lookup"><span data-stu-id="2f788-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f788-163">要求</span><span class="sxs-lookup"><span data-stu-id="2f788-163">Request</span></span>
<span data-ttu-id="2f788-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2f788-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
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

### <a name="response"></a><span data-ttu-id="2f788-165">応答</span><span class="sxs-lookup"><span data-stu-id="2f788-165">Response</span></span>
<span data-ttu-id="2f788-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2f788-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






