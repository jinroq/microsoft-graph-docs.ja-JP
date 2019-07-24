---
title: WindowsUpdateState の更新
description: WindowsUpdateState オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f003e5066e0e2b31b1b629067ffacc92efdd36de
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726111"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="d3c88-103">WindowsUpdateState の更新</span><span class="sxs-lookup"><span data-stu-id="d3c88-103">Update windowsUpdateState</span></span>

> <span data-ttu-id="d3c88-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3c88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3c88-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3c88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3c88-106">[WindowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d3c88-106">Update the properties of a [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3c88-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d3c88-107">Prerequisites</span></span>
<span data-ttu-id="d3c88-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3c88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3c88-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d3c88-110">Permission type</span></span>|<span data-ttu-id="d3c88-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d3c88-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3c88-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d3c88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d3c88-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3c88-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3c88-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d3c88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3c88-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3c88-115">Not supported.</span></span>|
|<span data-ttu-id="d3c88-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d3c88-116">Application</span></span>|<span data-ttu-id="d3c88-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3c88-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3c88-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d3c88-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="d3c88-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3c88-119">Request headers</span></span>
|<span data-ttu-id="d3c88-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3c88-120">Header</span></span>|<span data-ttu-id="d3c88-121">値</span><span class="sxs-lookup"><span data-stu-id="d3c88-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3c88-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3c88-122">Authorization</span></span>|<span data-ttu-id="d3c88-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3c88-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3c88-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d3c88-124">Accept</span></span>|<span data-ttu-id="d3c88-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3c88-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3c88-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d3c88-126">Request body</span></span>
<span data-ttu-id="d3c88-127">要求本文で、 [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d3c88-127">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="d3c88-128">次の表に、 [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d3c88-128">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md).</span></span>

|<span data-ttu-id="d3c88-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3c88-129">Property</span></span>|<span data-ttu-id="d3c88-130">型</span><span class="sxs-lookup"><span data-stu-id="d3c88-130">Type</span></span>|<span data-ttu-id="d3c88-131">説明</span><span class="sxs-lookup"><span data-stu-id="d3c88-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3c88-132">id</span><span class="sxs-lookup"><span data-stu-id="d3c88-132">id</span></span>|<span data-ttu-id="d3c88-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d3c88-133">String</span></span>|<span data-ttu-id="d3c88-134">これはエンティティの Id です。</span><span class="sxs-lookup"><span data-stu-id="d3c88-134">This is Id of the entity.</span></span>|
|<span data-ttu-id="d3c88-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="d3c88-135">deviceId</span></span>|<span data-ttu-id="d3c88-136">String</span><span class="sxs-lookup"><span data-stu-id="d3c88-136">String</span></span>|<span data-ttu-id="d3c88-137">デバイスの id。</span><span class="sxs-lookup"><span data-stu-id="d3c88-137">The id of the device.</span></span>|
|<span data-ttu-id="d3c88-138">userId</span><span class="sxs-lookup"><span data-stu-id="d3c88-138">userId</span></span>|<span data-ttu-id="d3c88-139">String</span><span class="sxs-lookup"><span data-stu-id="d3c88-139">String</span></span>|<span data-ttu-id="d3c88-140">ユーザーの id。</span><span class="sxs-lookup"><span data-stu-id="d3c88-140">The id of the user.</span></span>|
|<span data-ttu-id="d3c88-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d3c88-141">deviceDisplayName</span></span>|<span data-ttu-id="d3c88-142">String</span><span class="sxs-lookup"><span data-stu-id="d3c88-142">String</span></span>|<span data-ttu-id="d3c88-143">デバイスの表示名。</span><span class="sxs-lookup"><span data-stu-id="d3c88-143">Device display name.</span></span>|
|<span data-ttu-id="d3c88-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d3c88-144">userPrincipalName</span></span>|<span data-ttu-id="d3c88-145">String</span><span class="sxs-lookup"><span data-stu-id="d3c88-145">String</span></span>|<span data-ttu-id="d3c88-146">ユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="d3c88-146">User principal name.</span></span>|
|<span data-ttu-id="d3c88-147">status</span><span class="sxs-lookup"><span data-stu-id="d3c88-147">status</span></span>|[<span data-ttu-id="d3c88-148">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="d3c88-148">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="d3c88-149">Windows udpate 状態。</span><span class="sxs-lookup"><span data-stu-id="d3c88-149">Windows udpate status.</span></span> <span data-ttu-id="d3c88-150">使用可能な値は、`upToDate`、`pendingInstallation`、`pendingReboot`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="d3c88-150">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="d3c88-151">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="d3c88-151">qualityUpdateVersion</span></span>|<span data-ttu-id="d3c88-152">String</span><span class="sxs-lookup"><span data-stu-id="d3c88-152">String</span></span>|<span data-ttu-id="d3c88-153">デバイスの品質更新プログラムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d3c88-153">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="d3c88-154">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="d3c88-154">featureUpdateVersion</span></span>|<span data-ttu-id="d3c88-155">String</span><span class="sxs-lookup"><span data-stu-id="d3c88-155">String</span></span>|<span data-ttu-id="d3c88-156">デバイスの現在の機能更新バージョン。</span><span class="sxs-lookup"><span data-stu-id="d3c88-156">The current feature update version of the device.</span></span>|
|<span data-ttu-id="d3c88-157">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="d3c88-157">lastScanDateTime</span></span>|<span data-ttu-id="d3c88-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3c88-158">DateTimeOffset</span></span>|<span data-ttu-id="d3c88-159">Windows Update エージェントがスキャンに成功した日時。</span><span class="sxs-lookup"><span data-stu-id="d3c88-159">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="d3c88-160">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d3c88-160">lastSyncDateTime</span></span>|<span data-ttu-id="d3c88-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3c88-161">DateTimeOffset</span></span>|<span data-ttu-id="d3c88-162">デバイスと Microsoft Intune との同期が最後に実行された日時。</span><span class="sxs-lookup"><span data-stu-id="d3c88-162">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="d3c88-163">応答</span><span class="sxs-lookup"><span data-stu-id="d3c88-163">Response</span></span>
<span data-ttu-id="d3c88-164">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d3c88-164">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3c88-165">例</span><span class="sxs-lookup"><span data-stu-id="d3c88-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3c88-166">要求</span><span class="sxs-lookup"><span data-stu-id="d3c88-166">Request</span></span>
<span data-ttu-id="d3c88-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d3c88-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
Content-type: application/json
Content-length: 504

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a><span data-ttu-id="d3c88-168">応答</span><span class="sxs-lookup"><span data-stu-id="d3c88-168">Response</span></span>
<span data-ttu-id="d3c88-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d3c88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "id": "3d92af00-af00-3d92-00af-923d00af923d",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```




