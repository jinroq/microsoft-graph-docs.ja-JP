---
title: deviceInstallState の作成
description: 新しい deviceInstallState オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 244a03aa7c1f42c6e71591a3358ab7fca67a9b48
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853887"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="4e699-103">deviceInstallState の作成</span><span class="sxs-lookup"><span data-stu-id="4e699-103">Create deviceInstallState</span></span>

> <span data-ttu-id="4e699-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4e699-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e699-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e699-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e699-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4e699-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e699-107">新しい [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4e699-107">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e699-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4e699-108">Prerequisites</span></span>
<span data-ttu-id="4e699-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e699-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e699-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4e699-111">Permission type</span></span>|<span data-ttu-id="4e699-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4e699-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e699-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4e699-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e699-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e699-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e699-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4e699-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e699-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e699-116">Not supported.</span></span>|
|<span data-ttu-id="4e699-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4e699-117">Application</span></span>|<span data-ttu-id="4e699-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e699-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e699-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4e699-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="4e699-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e699-120">Request headers</span></span>
|<span data-ttu-id="4e699-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e699-121">Header</span></span>|<span data-ttu-id="4e699-122">値</span><span class="sxs-lookup"><span data-stu-id="4e699-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e699-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e699-123">Authorization</span></span>|<span data-ttu-id="4e699-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4e699-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e699-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e699-125">Accept</span></span>|<span data-ttu-id="4e699-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e699-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e699-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4e699-127">Request body</span></span>
<span data-ttu-id="4e699-128">要求本文で、deviceInstallState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e699-128">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="4e699-129">次の表に、deviceInstallState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4e699-129">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="4e699-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e699-130">Property</span></span>|<span data-ttu-id="4e699-131">種類</span><span class="sxs-lookup"><span data-stu-id="4e699-131">Type</span></span>|<span data-ttu-id="4e699-132">説明</span><span class="sxs-lookup"><span data-stu-id="4e699-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e699-133">ID</span><span class="sxs-lookup"><span data-stu-id="4e699-133">id</span></span>|<span data-ttu-id="4e699-134">String</span><span class="sxs-lookup"><span data-stu-id="4e699-134">String</span></span>|<span data-ttu-id="4e699-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4e699-135">Key of the entity.</span></span>|
|<span data-ttu-id="4e699-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="4e699-136">deviceName</span></span>|<span data-ttu-id="4e699-137">String</span><span class="sxs-lookup"><span data-stu-id="4e699-137">String</span></span>|<span data-ttu-id="4e699-138">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="4e699-138">Device name.</span></span>|
|<span data-ttu-id="4e699-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="4e699-139">deviceId</span></span>|<span data-ttu-id="4e699-140">String</span><span class="sxs-lookup"><span data-stu-id="4e699-140">String</span></span>|<span data-ttu-id="4e699-141">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="4e699-141">Device Id.</span></span>|
|<span data-ttu-id="4e699-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4e699-142">lastSyncDateTime</span></span>|<span data-ttu-id="4e699-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e699-143">DateTimeOffset</span></span>|<span data-ttu-id="4e699-144">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="4e699-144">Last sync date and time.</span></span>|
|<span data-ttu-id="4e699-145">installState</span><span class="sxs-lookup"><span data-stu-id="4e699-145">installState</span></span>|[<span data-ttu-id="4e699-146">installState</span><span class="sxs-lookup"><span data-stu-id="4e699-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="4e699-147">電子ブックのインストールの状態。</span><span class="sxs-lookup"><span data-stu-id="4e699-147">The install state of the eBook.</span></span> <span data-ttu-id="4e699-148">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="4e699-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="4e699-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="4e699-149">errorCode</span></span>|<span data-ttu-id="4e699-150">String</span><span class="sxs-lookup"><span data-stu-id="4e699-150">String</span></span>|<span data-ttu-id="4e699-151">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="4e699-151">The error code for install failures.</span></span>|
|<span data-ttu-id="4e699-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="4e699-152">osVersion</span></span>|<span data-ttu-id="4e699-153">String</span><span class="sxs-lookup"><span data-stu-id="4e699-153">String</span></span>|<span data-ttu-id="4e699-154">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="4e699-154">OS Version.</span></span>|
|<span data-ttu-id="4e699-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="4e699-155">osDescription</span></span>|<span data-ttu-id="4e699-156">String</span><span class="sxs-lookup"><span data-stu-id="4e699-156">String</span></span>|<span data-ttu-id="4e699-157">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="4e699-157">OS Description.</span></span>|
|<span data-ttu-id="4e699-158">userName</span><span class="sxs-lookup"><span data-stu-id="4e699-158">userName</span></span>|<span data-ttu-id="4e699-159">String</span><span class="sxs-lookup"><span data-stu-id="4e699-159">String</span></span>|<span data-ttu-id="4e699-160">デバイスのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="4e699-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="4e699-161">応答</span><span class="sxs-lookup"><span data-stu-id="4e699-161">Response</span></span>
<span data-ttu-id="4e699-162">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4e699-162">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e699-163">例</span><span class="sxs-lookup"><span data-stu-id="4e699-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e699-164">要求</span><span class="sxs-lookup"><span data-stu-id="4e699-164">Request</span></span>
<span data-ttu-id="4e699-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4e699-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4e699-166">応答</span><span class="sxs-lookup"><span data-stu-id="4e699-166">Response</span></span>
<span data-ttu-id="4e699-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4e699-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





