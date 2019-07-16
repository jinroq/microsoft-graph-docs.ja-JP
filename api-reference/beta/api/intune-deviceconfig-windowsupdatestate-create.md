---
title: WindowsUpdateState を作成する
description: 新しい windowsUpdateState オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b428197cea201bffc59153d3df561ea7ddacea4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726080"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="f90c3-103">WindowsUpdateState を作成する</span><span class="sxs-lookup"><span data-stu-id="f90c3-103">Create windowsUpdateState</span></span>

> <span data-ttu-id="f90c3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f90c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f90c3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f90c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f90c3-106">新しい[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f90c3-106">Create a new [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f90c3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f90c3-107">Prerequisites</span></span>
<span data-ttu-id="f90c3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f90c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f90c3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f90c3-110">Permission type</span></span>|<span data-ttu-id="f90c3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f90c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f90c3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f90c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f90c3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f90c3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f90c3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f90c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f90c3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f90c3-115">Not supported.</span></span>|
|<span data-ttu-id="f90c3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f90c3-116">Application</span></span>|<span data-ttu-id="f90c3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f90c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f90c3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f90c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="f90c3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f90c3-119">Request headers</span></span>
|<span data-ttu-id="f90c3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f90c3-120">Header</span></span>|<span data-ttu-id="f90c3-121">値</span><span class="sxs-lookup"><span data-stu-id="f90c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f90c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f90c3-122">Authorization</span></span>|<span data-ttu-id="f90c3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f90c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f90c3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f90c3-124">Accept</span></span>|<span data-ttu-id="f90c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f90c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f90c3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f90c3-126">Request body</span></span>
<span data-ttu-id="f90c3-127">要求本文で、windowsUpdateState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f90c3-127">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="f90c3-128">次の表に、windowsUpdateState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f90c3-128">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="f90c3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f90c3-129">Property</span></span>|<span data-ttu-id="f90c3-130">型</span><span class="sxs-lookup"><span data-stu-id="f90c3-130">Type</span></span>|<span data-ttu-id="f90c3-131">説明</span><span class="sxs-lookup"><span data-stu-id="f90c3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f90c3-132">id</span><span class="sxs-lookup"><span data-stu-id="f90c3-132">id</span></span>|<span data-ttu-id="f90c3-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f90c3-133">String</span></span>|<span data-ttu-id="f90c3-134">これはエンティティの Id です。</span><span class="sxs-lookup"><span data-stu-id="f90c3-134">This is Id of the entity.</span></span>|
|<span data-ttu-id="f90c3-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="f90c3-135">deviceId</span></span>|<span data-ttu-id="f90c3-136">String</span><span class="sxs-lookup"><span data-stu-id="f90c3-136">String</span></span>|<span data-ttu-id="f90c3-137">デバイスの id。</span><span class="sxs-lookup"><span data-stu-id="f90c3-137">The id of the device.</span></span>|
|<span data-ttu-id="f90c3-138">userId</span><span class="sxs-lookup"><span data-stu-id="f90c3-138">userId</span></span>|<span data-ttu-id="f90c3-139">String</span><span class="sxs-lookup"><span data-stu-id="f90c3-139">String</span></span>|<span data-ttu-id="f90c3-140">ユーザーの id。</span><span class="sxs-lookup"><span data-stu-id="f90c3-140">The id of the user.</span></span>|
|<span data-ttu-id="f90c3-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f90c3-141">deviceDisplayName</span></span>|<span data-ttu-id="f90c3-142">String</span><span class="sxs-lookup"><span data-stu-id="f90c3-142">String</span></span>|<span data-ttu-id="f90c3-143">デバイスの表示名。</span><span class="sxs-lookup"><span data-stu-id="f90c3-143">Device display name.</span></span>|
|<span data-ttu-id="f90c3-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f90c3-144">userPrincipalName</span></span>|<span data-ttu-id="f90c3-145">String</span><span class="sxs-lookup"><span data-stu-id="f90c3-145">String</span></span>|<span data-ttu-id="f90c3-146">ユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="f90c3-146">User principal name.</span></span>|
|<span data-ttu-id="f90c3-147">status</span><span class="sxs-lookup"><span data-stu-id="f90c3-147">status</span></span>|[<span data-ttu-id="f90c3-148">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="f90c3-148">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="f90c3-149">Windows udpate 状態。</span><span class="sxs-lookup"><span data-stu-id="f90c3-149">Windows udpate status.</span></span> <span data-ttu-id="f90c3-150">使用可能な値は、`upToDate`、`pendingInstallation`、`pendingReboot`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="f90c3-150">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="f90c3-151">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="f90c3-151">qualityUpdateVersion</span></span>|<span data-ttu-id="f90c3-152">String</span><span class="sxs-lookup"><span data-stu-id="f90c3-152">String</span></span>|<span data-ttu-id="f90c3-153">デバイスの品質更新プログラムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f90c3-153">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="f90c3-154">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="f90c3-154">featureUpdateVersion</span></span>|<span data-ttu-id="f90c3-155">String</span><span class="sxs-lookup"><span data-stu-id="f90c3-155">String</span></span>|<span data-ttu-id="f90c3-156">デバイスの現在の機能更新バージョン。</span><span class="sxs-lookup"><span data-stu-id="f90c3-156">The current feature update version of the device.</span></span>|
|<span data-ttu-id="f90c3-157">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="f90c3-157">lastScanDateTime</span></span>|<span data-ttu-id="f90c3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f90c3-158">DateTimeOffset</span></span>|<span data-ttu-id="f90c3-159">Windows Update エージェントがスキャンに成功した日時。</span><span class="sxs-lookup"><span data-stu-id="f90c3-159">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="f90c3-160">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f90c3-160">lastSyncDateTime</span></span>|<span data-ttu-id="f90c3-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f90c3-161">DateTimeOffset</span></span>|<span data-ttu-id="f90c3-162">デバイスと Microsoft Intune との同期が最後に実行された日時。</span><span class="sxs-lookup"><span data-stu-id="f90c3-162">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="f90c3-163">応答</span><span class="sxs-lookup"><span data-stu-id="f90c3-163">Response</span></span>
<span data-ttu-id="f90c3-164">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f90c3-164">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f90c3-165">例</span><span class="sxs-lookup"><span data-stu-id="f90c3-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="f90c3-166">要求</span><span class="sxs-lookup"><span data-stu-id="f90c3-166">Request</span></span>
<span data-ttu-id="f90c3-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f90c3-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
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

### <a name="response"></a><span data-ttu-id="f90c3-168">応答</span><span class="sxs-lookup"><span data-stu-id="f90c3-168">Response</span></span>
<span data-ttu-id="f90c3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f90c3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





