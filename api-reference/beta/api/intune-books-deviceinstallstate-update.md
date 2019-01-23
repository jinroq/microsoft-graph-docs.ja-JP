---
title: deviceInstallState の更新
description: deviceInstallState オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d73f1cc881d918f385bfdc8d98cf9a1451a554e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394790"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="f3759-103">deviceInstallState の更新</span><span class="sxs-lookup"><span data-stu-id="f3759-103">Update deviceInstallState</span></span>

> <span data-ttu-id="f3759-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f3759-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f3759-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3759-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3759-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3759-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3759-107">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f3759-107">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3759-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f3759-108">Prerequisites</span></span>
<span data-ttu-id="f3759-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3759-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f3759-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3759-111">Permission type</span></span>|<span data-ttu-id="f3759-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3759-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3759-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3759-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3759-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3759-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3759-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3759-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3759-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3759-116">Not supported.</span></span>|
|<span data-ttu-id="f3759-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3759-117">Application</span></span>|<span data-ttu-id="f3759-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3759-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3759-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3759-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="f3759-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3759-120">Request headers</span></span>
|<span data-ttu-id="f3759-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3759-121">Header</span></span>|<span data-ttu-id="f3759-122">値</span><span class="sxs-lookup"><span data-stu-id="f3759-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3759-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3759-123">Authorization</span></span>|<span data-ttu-id="f3759-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f3759-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3759-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3759-125">Accept</span></span>|<span data-ttu-id="f3759-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3759-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3759-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3759-127">Request body</span></span>
<span data-ttu-id="f3759-128">要求本文で、[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3759-128">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="f3759-129">次の表に、[deviceInstallState](../resources/intune-books-deviceinstallstate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f3759-129">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="f3759-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3759-130">Property</span></span>|<span data-ttu-id="f3759-131">型</span><span class="sxs-lookup"><span data-stu-id="f3759-131">Type</span></span>|<span data-ttu-id="f3759-132">説明</span><span class="sxs-lookup"><span data-stu-id="f3759-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3759-133">id</span><span class="sxs-lookup"><span data-stu-id="f3759-133">id</span></span>|<span data-ttu-id="f3759-134">String</span><span class="sxs-lookup"><span data-stu-id="f3759-134">String</span></span>|<span data-ttu-id="f3759-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f3759-135">Key of the entity.</span></span>|
|<span data-ttu-id="f3759-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="f3759-136">deviceName</span></span>|<span data-ttu-id="f3759-137">String</span><span class="sxs-lookup"><span data-stu-id="f3759-137">String</span></span>|<span data-ttu-id="f3759-138">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="f3759-138">Device name.</span></span>|
|<span data-ttu-id="f3759-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="f3759-139">deviceId</span></span>|<span data-ttu-id="f3759-140">String</span><span class="sxs-lookup"><span data-stu-id="f3759-140">String</span></span>|<span data-ttu-id="f3759-141">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="f3759-141">Device Id.</span></span>|
|<span data-ttu-id="f3759-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f3759-142">lastSyncDateTime</span></span>|<span data-ttu-id="f3759-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3759-143">DateTimeOffset</span></span>|<span data-ttu-id="f3759-144">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="f3759-144">Last sync date and time.</span></span>|
|<span data-ttu-id="f3759-145">installState</span><span class="sxs-lookup"><span data-stu-id="f3759-145">installState</span></span>|[<span data-ttu-id="f3759-146">installState</span><span class="sxs-lookup"><span data-stu-id="f3759-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="f3759-147">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="f3759-147">The install state of the eBook.</span></span> <span data-ttu-id="f3759-148">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="f3759-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="f3759-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="f3759-149">errorCode</span></span>|<span data-ttu-id="f3759-150">String</span><span class="sxs-lookup"><span data-stu-id="f3759-150">String</span></span>|<span data-ttu-id="f3759-151">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="f3759-151">The error code for install failures.</span></span>|
|<span data-ttu-id="f3759-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="f3759-152">osVersion</span></span>|<span data-ttu-id="f3759-153">String</span><span class="sxs-lookup"><span data-stu-id="f3759-153">String</span></span>|<span data-ttu-id="f3759-154">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="f3759-154">OS Version.</span></span>|
|<span data-ttu-id="f3759-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="f3759-155">osDescription</span></span>|<span data-ttu-id="f3759-156">String</span><span class="sxs-lookup"><span data-stu-id="f3759-156">String</span></span>|<span data-ttu-id="f3759-157">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="f3759-157">OS Description.</span></span>|
|<span data-ttu-id="f3759-158">userName</span><span class="sxs-lookup"><span data-stu-id="f3759-158">userName</span></span>|<span data-ttu-id="f3759-159">String</span><span class="sxs-lookup"><span data-stu-id="f3759-159">String</span></span>|<span data-ttu-id="f3759-160">デバイスのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="f3759-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="f3759-161">応答</span><span class="sxs-lookup"><span data-stu-id="f3759-161">Response</span></span>
<span data-ttu-id="f3759-162">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3759-162">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3759-163">例</span><span class="sxs-lookup"><span data-stu-id="f3759-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3759-164">要求</span><span class="sxs-lookup"><span data-stu-id="f3759-164">Request</span></span>
<span data-ttu-id="f3759-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3759-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f3759-166">応答</span><span class="sxs-lookup"><span data-stu-id="f3759-166">Response</span></span>
<span data-ttu-id="f3759-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3759-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




