---
title: DepOnboardingSetting の更新
description: DepOnboardingSetting オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1187cf203b897d76feaeedb6cbb484f71ab46b07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985281"
---
# <a name="update-deponboardingsetting"></a><span data-ttu-id="8cc60-103">DepOnboardingSetting の更新</span><span class="sxs-lookup"><span data-stu-id="8cc60-103">Update depOnboardingSetting</span></span>

> <span data-ttu-id="8cc60-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cc60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cc60-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8cc60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cc60-106">[Deponboardingsetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8cc60-106">Update the properties of a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cc60-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8cc60-107">Prerequisites</span></span>
<span data-ttu-id="8cc60-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8cc60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc60-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8cc60-110">Permission type</span></span>|<span data-ttu-id="8cc60-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8cc60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cc60-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8cc60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8cc60-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc60-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8cc60-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8cc60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cc60-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cc60-115">Not supported.</span></span>|
|<span data-ttu-id="8cc60-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8cc60-116">Application</span></span>|<span data-ttu-id="8cc60-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cc60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cc60-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8cc60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="8cc60-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cc60-119">Request headers</span></span>
|<span data-ttu-id="8cc60-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cc60-120">Header</span></span>|<span data-ttu-id="8cc60-121">値</span><span class="sxs-lookup"><span data-stu-id="8cc60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cc60-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cc60-122">Authorization</span></span>|<span data-ttu-id="8cc60-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8cc60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cc60-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8cc60-124">Accept</span></span>|<span data-ttu-id="8cc60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8cc60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cc60-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8cc60-126">Request body</span></span>
<span data-ttu-id="8cc60-127">要求本文で、 [Deponboardingsetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8cc60-127">In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

<span data-ttu-id="8cc60-128">次の表に、 [Deponboardingsetting](../resources/intune-enrollment-deponboardingsetting.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8cc60-128">The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span></span>

|<span data-ttu-id="8cc60-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cc60-129">Property</span></span>|<span data-ttu-id="8cc60-130">型</span><span class="sxs-lookup"><span data-stu-id="8cc60-130">Type</span></span>|<span data-ttu-id="8cc60-131">説明</span><span class="sxs-lookup"><span data-stu-id="8cc60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc60-132">id</span><span class="sxs-lookup"><span data-stu-id="8cc60-132">id</span></span>|<span data-ttu-id="8cc60-133">String</span><span class="sxs-lookup"><span data-stu-id="8cc60-133">String</span></span>|<span data-ttu-id="8cc60-134">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="8cc60-134">UUID for the object</span></span>|
|<span data-ttu-id="8cc60-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="8cc60-135">appleIdentifier</span></span>|<span data-ttu-id="8cc60-136">String</span><span class="sxs-lookup"><span data-stu-id="8cc60-136">String</span></span>|<span data-ttu-id="8cc60-137">現在のトークンを取得するために使用される Apple ID。</span><span class="sxs-lookup"><span data-stu-id="8cc60-137">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="8cc60-138">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc60-138">tokenExpirationDateTime</span></span>|<span data-ttu-id="8cc60-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc60-139">DateTimeOffset</span></span>|<span data-ttu-id="8cc60-140">トークンの有効期限が切れるとき。</span><span class="sxs-lookup"><span data-stu-id="8cc60-140">When the token will expire.</span></span>|
|<span data-ttu-id="8cc60-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc60-141">lastModifiedDateTime</span></span>|<span data-ttu-id="8cc60-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc60-142">DateTimeOffset</span></span>|<span data-ttu-id="8cc60-143">サービスが利用されたとき。</span><span class="sxs-lookup"><span data-stu-id="8cc60-143">When the service was onboarded.</span></span>|
|<span data-ttu-id="8cc60-144">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc60-144">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="8cc60-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc60-145">DateTimeOffset</span></span>|<span data-ttu-id="8cc60-146">Intune でサービスが最後に使用されたとき</span><span class="sxs-lookup"><span data-stu-id="8cc60-146">When the service last syned with Intune</span></span>|
|<span data-ttu-id="8cc60-147">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc60-147">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="8cc60-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc60-148">DateTimeOffset</span></span>|<span data-ttu-id="8cc60-149">Intune が最後に同期を要求したとき。</span><span class="sxs-lookup"><span data-stu-id="8cc60-149">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="8cc60-150">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="8cc60-150">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="8cc60-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc60-151">Boolean</span></span>|<span data-ttu-id="8cc60-152">School Data Sync サービスで Dep トークンの共有が有効になっているかどうか。</span><span class="sxs-lookup"><span data-stu-id="8cc60-152">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="8cc60-153">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="8cc60-153">lastSyncErrorCode</span></span>|<span data-ttu-id="8cc60-154">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc60-154">Int32</span></span>|<span data-ttu-id="8cc60-155">前回の dep 同期中に Apple によって報告されたエラーコード。</span><span class="sxs-lookup"><span data-stu-id="8cc60-155">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="8cc60-156">tokenType</span><span class="sxs-lookup"><span data-stu-id="8cc60-156">tokenType</span></span>|[<span data-ttu-id="8cc60-157">depTokenType</span><span class="sxs-lookup"><span data-stu-id="8cc60-157">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="8cc60-158">Dep トークンの種類を取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="8cc60-158">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="8cc60-159">可能な値は、`none`、`dep`、`appleSchoolManager` です。</span><span class="sxs-lookup"><span data-stu-id="8cc60-159">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="8cc60-160">tokenName</span><span class="sxs-lookup"><span data-stu-id="8cc60-160">tokenName</span></span>|<span data-ttu-id="8cc60-161">String</span><span class="sxs-lookup"><span data-stu-id="8cc60-161">String</span></span>|<span data-ttu-id="8cc60-162">Dep トークンのフレンドリ名</span><span class="sxs-lookup"><span data-stu-id="8cc60-162">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="8cc60-163">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8cc60-163">syncedDeviceCount</span></span>|<span data-ttu-id="8cc60-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc60-164">Int32</span></span>|<span data-ttu-id="8cc60-165">同期されたデバイスの数を取得する</span><span class="sxs-lookup"><span data-stu-id="8cc60-165">Gets synced device count</span></span>|
|<span data-ttu-id="8cc60-166">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="8cc60-166">dataSharingConsentGranted</span></span>|<span data-ttu-id="8cc60-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc60-167">Boolean</span></span>|<span data-ttu-id="8cc60-168">Apple Dep サービスでのデータ共有に対して付与される同意</span><span class="sxs-lookup"><span data-stu-id="8cc60-168">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="8cc60-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8cc60-169">roleScopeTagIds</span></span>|<span data-ttu-id="8cc60-170">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8cc60-170">String collection</span></span>|<span data-ttu-id="8cc60-171">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="8cc60-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="8cc60-172">応答</span><span class="sxs-lookup"><span data-stu-id="8cc60-172">Response</span></span>
<span data-ttu-id="8cc60-173">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Deponboardingsetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8cc60-173">If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc60-174">例</span><span class="sxs-lookup"><span data-stu-id="8cc60-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cc60-175">要求</span><span class="sxs-lookup"><span data-stu-id="8cc60-175">Request</span></span>
<span data-ttu-id="8cc60-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8cc60-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 576

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="8cc60-177">応答</span><span class="sxs-lookup"><span data-stu-id="8cc60-177">Response</span></span>
<span data-ttu-id="8cc60-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8cc60-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 689

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "40342229-2229-4034-2922-344029223440",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





