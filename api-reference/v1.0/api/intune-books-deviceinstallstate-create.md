---
title: deviceInstallState の作成
description: 新しい deviceInstallState オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03eeaaedcb4c4d5d6b1fee6077ab623cab946290
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263589"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="835f2-103">deviceInstallState の作成</span><span class="sxs-lookup"><span data-stu-id="835f2-103">Create deviceInstallState</span></span>

> <span data-ttu-id="835f2-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="835f2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="835f2-105">新しい [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="835f2-105">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="835f2-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="835f2-106">Prerequisites</span></span>
<span data-ttu-id="835f2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="835f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="835f2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="835f2-109">Permission type</span></span>|<span data-ttu-id="835f2-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="835f2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="835f2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="835f2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="835f2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="835f2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="835f2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="835f2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="835f2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="835f2-114">Not supported.</span></span>|
|<span data-ttu-id="835f2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="835f2-115">Application</span></span>|<span data-ttu-id="835f2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="835f2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="835f2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="835f2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="835f2-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="835f2-118">Request headers</span></span>
|<span data-ttu-id="835f2-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="835f2-119">Header</span></span>|<span data-ttu-id="835f2-120">値</span><span class="sxs-lookup"><span data-stu-id="835f2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="835f2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="835f2-121">Authorization</span></span>|<span data-ttu-id="835f2-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="835f2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="835f2-123">承諾</span><span class="sxs-lookup"><span data-stu-id="835f2-123">Accept</span></span>|<span data-ttu-id="835f2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="835f2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="835f2-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="835f2-125">Request body</span></span>
<span data-ttu-id="835f2-126">要求本文で、deviceInstallState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="835f2-126">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="835f2-127">次の表に、deviceInstallState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="835f2-127">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="835f2-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="835f2-128">Property</span></span>|<span data-ttu-id="835f2-129">型</span><span class="sxs-lookup"><span data-stu-id="835f2-129">Type</span></span>|<span data-ttu-id="835f2-130">説明</span><span class="sxs-lookup"><span data-stu-id="835f2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="835f2-131">id</span><span class="sxs-lookup"><span data-stu-id="835f2-131">id</span></span>|<span data-ttu-id="835f2-132">文字列</span><span class="sxs-lookup"><span data-stu-id="835f2-132">String</span></span>|<span data-ttu-id="835f2-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="835f2-133">Key of the entity.</span></span>|
|<span data-ttu-id="835f2-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="835f2-134">deviceName</span></span>|<span data-ttu-id="835f2-135">String</span><span class="sxs-lookup"><span data-stu-id="835f2-135">String</span></span>|<span data-ttu-id="835f2-136">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="835f2-136">Device name.</span></span>|
|<span data-ttu-id="835f2-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="835f2-137">deviceId</span></span>|<span data-ttu-id="835f2-138">String</span><span class="sxs-lookup"><span data-stu-id="835f2-138">String</span></span>|<span data-ttu-id="835f2-139">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="835f2-139">Device Id.</span></span>|
|<span data-ttu-id="835f2-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="835f2-140">lastSyncDateTime</span></span>|<span data-ttu-id="835f2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="835f2-141">DateTimeOffset</span></span>|<span data-ttu-id="835f2-142">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="835f2-142">Last sync date and time.</span></span>|
|<span data-ttu-id="835f2-143">installState</span><span class="sxs-lookup"><span data-stu-id="835f2-143">installState</span></span>|[<span data-ttu-id="835f2-144">installState</span><span class="sxs-lookup"><span data-stu-id="835f2-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="835f2-145">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="835f2-145">The install state of the eBook.</span></span> <span data-ttu-id="835f2-146">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="835f2-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="835f2-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="835f2-147">errorCode</span></span>|<span data-ttu-id="835f2-148">String</span><span class="sxs-lookup"><span data-stu-id="835f2-148">String</span></span>|<span data-ttu-id="835f2-149">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="835f2-149">The error code for install failures.</span></span>|
|<span data-ttu-id="835f2-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="835f2-150">osVersion</span></span>|<span data-ttu-id="835f2-151">String</span><span class="sxs-lookup"><span data-stu-id="835f2-151">String</span></span>|<span data-ttu-id="835f2-152">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="835f2-152">OS Version.</span></span>|
|<span data-ttu-id="835f2-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="835f2-153">osDescription</span></span>|<span data-ttu-id="835f2-154">String</span><span class="sxs-lookup"><span data-stu-id="835f2-154">String</span></span>|<span data-ttu-id="835f2-155">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="835f2-155">OS Description.</span></span>|
|<span data-ttu-id="835f2-156">userName</span><span class="sxs-lookup"><span data-stu-id="835f2-156">userName</span></span>|<span data-ttu-id="835f2-157">String</span><span class="sxs-lookup"><span data-stu-id="835f2-157">String</span></span>|<span data-ttu-id="835f2-158">デバイスのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="835f2-158">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="835f2-159">応答</span><span class="sxs-lookup"><span data-stu-id="835f2-159">Response</span></span>
<span data-ttu-id="835f2-160">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="835f2-160">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="835f2-161">例</span><span class="sxs-lookup"><span data-stu-id="835f2-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="835f2-162">要求</span><span class="sxs-lookup"><span data-stu-id="835f2-162">Request</span></span>
<span data-ttu-id="835f2-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="835f2-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
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

### <a name="response"></a><span data-ttu-id="835f2-164">応答</span><span class="sxs-lookup"><span data-stu-id="835f2-164">Response</span></span>
<span data-ttu-id="835f2-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="835f2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



