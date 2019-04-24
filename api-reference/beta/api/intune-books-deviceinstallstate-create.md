---
title: deviceInstallState の作成
description: 新しい deviceInstallState オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16af56e2bf82b5e15d259229ae9a2416fa20e92c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32484039"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="2bccc-103">deviceInstallState の作成</span><span class="sxs-lookup"><span data-stu-id="2bccc-103">Create deviceInstallState</span></span>

> <span data-ttu-id="2bccc-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bccc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bccc-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2bccc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bccc-106">新しい [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2bccc-106">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bccc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2bccc-107">Prerequisites</span></span>
<span data-ttu-id="2bccc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2bccc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bccc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2bccc-110">Permission type</span></span>|<span data-ttu-id="2bccc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2bccc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bccc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2bccc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2bccc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bccc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2bccc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2bccc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bccc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bccc-115">Not supported.</span></span>|
|<span data-ttu-id="2bccc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2bccc-116">Application</span></span>|<span data-ttu-id="2bccc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bccc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bccc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2bccc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="2bccc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2bccc-119">Request headers</span></span>
|<span data-ttu-id="2bccc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2bccc-120">Header</span></span>|<span data-ttu-id="2bccc-121">値</span><span class="sxs-lookup"><span data-stu-id="2bccc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bccc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bccc-122">Authorization</span></span>|<span data-ttu-id="2bccc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2bccc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bccc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2bccc-124">Accept</span></span>|<span data-ttu-id="2bccc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2bccc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bccc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2bccc-126">Request body</span></span>
<span data-ttu-id="2bccc-127">要求本文で、deviceInstallState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2bccc-127">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="2bccc-128">次の表に、deviceInstallState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2bccc-128">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="2bccc-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2bccc-129">Property</span></span>|<span data-ttu-id="2bccc-130">型</span><span class="sxs-lookup"><span data-stu-id="2bccc-130">Type</span></span>|<span data-ttu-id="2bccc-131">説明</span><span class="sxs-lookup"><span data-stu-id="2bccc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bccc-132">id</span><span class="sxs-lookup"><span data-stu-id="2bccc-132">id</span></span>|<span data-ttu-id="2bccc-133">String</span><span class="sxs-lookup"><span data-stu-id="2bccc-133">String</span></span>|<span data-ttu-id="2bccc-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2bccc-134">Key of the entity.</span></span>|
|<span data-ttu-id="2bccc-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="2bccc-135">deviceName</span></span>|<span data-ttu-id="2bccc-136">String</span><span class="sxs-lookup"><span data-stu-id="2bccc-136">String</span></span>|<span data-ttu-id="2bccc-137">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="2bccc-137">Device name.</span></span>|
|<span data-ttu-id="2bccc-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="2bccc-138">deviceId</span></span>|<span data-ttu-id="2bccc-139">String</span><span class="sxs-lookup"><span data-stu-id="2bccc-139">String</span></span>|<span data-ttu-id="2bccc-140">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="2bccc-140">Device Id.</span></span>|
|<span data-ttu-id="2bccc-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2bccc-141">lastSyncDateTime</span></span>|<span data-ttu-id="2bccc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bccc-142">DateTimeOffset</span></span>|<span data-ttu-id="2bccc-143">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="2bccc-143">Last sync date and time.</span></span>|
|<span data-ttu-id="2bccc-144">installState</span><span class="sxs-lookup"><span data-stu-id="2bccc-144">installState</span></span>|[<span data-ttu-id="2bccc-145">installState</span><span class="sxs-lookup"><span data-stu-id="2bccc-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="2bccc-146">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="2bccc-146">The install state of the eBook.</span></span> <span data-ttu-id="2bccc-147">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="2bccc-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="2bccc-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="2bccc-148">errorCode</span></span>|<span data-ttu-id="2bccc-149">String</span><span class="sxs-lookup"><span data-stu-id="2bccc-149">String</span></span>|<span data-ttu-id="2bccc-150">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="2bccc-150">The error code for install failures.</span></span>|
|<span data-ttu-id="2bccc-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="2bccc-151">osVersion</span></span>|<span data-ttu-id="2bccc-152">String</span><span class="sxs-lookup"><span data-stu-id="2bccc-152">String</span></span>|<span data-ttu-id="2bccc-153">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="2bccc-153">OS Version.</span></span>|
|<span data-ttu-id="2bccc-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="2bccc-154">osDescription</span></span>|<span data-ttu-id="2bccc-155">String</span><span class="sxs-lookup"><span data-stu-id="2bccc-155">String</span></span>|<span data-ttu-id="2bccc-156">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="2bccc-156">OS Description.</span></span>|
|<span data-ttu-id="2bccc-157">userName</span><span class="sxs-lookup"><span data-stu-id="2bccc-157">userName</span></span>|<span data-ttu-id="2bccc-158">String</span><span class="sxs-lookup"><span data-stu-id="2bccc-158">String</span></span>|<span data-ttu-id="2bccc-159">デバイスのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="2bccc-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="2bccc-160">応答</span><span class="sxs-lookup"><span data-stu-id="2bccc-160">Response</span></span>
<span data-ttu-id="2bccc-161">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2bccc-161">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bccc-162">例</span><span class="sxs-lookup"><span data-stu-id="2bccc-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bccc-163">要求</span><span class="sxs-lookup"><span data-stu-id="2bccc-163">Request</span></span>
<span data-ttu-id="2bccc-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2bccc-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
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

### <a name="response"></a><span data-ttu-id="2bccc-165">応答</span><span class="sxs-lookup"><span data-stu-id="2bccc-165">Response</span></span>
<span data-ttu-id="2bccc-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2bccc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





