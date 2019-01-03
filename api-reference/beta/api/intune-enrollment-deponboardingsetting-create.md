---
title: DepOnboardingSetting を作成します。
description: 新しい depOnboardingSetting オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 11f2e5217e4040a7d4345c9271b459e608075498
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330661"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="3307a-103">DepOnboardingSetting を作成します。</span><span class="sxs-lookup"><span data-stu-id="3307a-103">Create depOnboardingSetting</span></span>

> <span data-ttu-id="3307a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3307a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3307a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3307a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3307a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3307a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3307a-107">新しい[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3307a-107">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3307a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3307a-108">Prerequisites</span></span>
<span data-ttu-id="3307a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3307a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3307a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3307a-111">Permission type</span></span>|<span data-ttu-id="3307a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3307a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3307a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3307a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3307a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3307a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3307a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3307a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3307a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3307a-116">Not supported.</span></span>|
|<span data-ttu-id="3307a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3307a-117">Application</span></span>|<span data-ttu-id="3307a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3307a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3307a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3307a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="3307a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3307a-120">Request headers</span></span>
|<span data-ttu-id="3307a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3307a-121">Header</span></span>|<span data-ttu-id="3307a-122">値</span><span class="sxs-lookup"><span data-stu-id="3307a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3307a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3307a-123">Authorization</span></span>|<span data-ttu-id="3307a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3307a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3307a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3307a-125">Accept</span></span>|<span data-ttu-id="3307a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3307a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3307a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3307a-127">Request body</span></span>
<span data-ttu-id="3307a-128">要求の本文に depOnboardingSetting オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="3307a-128">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="3307a-129">次の表は、depOnboardingSetting を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3307a-129">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="3307a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3307a-130">Property</span></span>|<span data-ttu-id="3307a-131">種類</span><span class="sxs-lookup"><span data-stu-id="3307a-131">Type</span></span>|<span data-ttu-id="3307a-132">説明</span><span class="sxs-lookup"><span data-stu-id="3307a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3307a-133">ID</span><span class="sxs-lookup"><span data-stu-id="3307a-133">id</span></span>|<span data-ttu-id="3307a-134">String</span><span class="sxs-lookup"><span data-stu-id="3307a-134">String</span></span>|<span data-ttu-id="3307a-135">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="3307a-135">UUID for the object</span></span>|
|<span data-ttu-id="3307a-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="3307a-136">appleIdentifier</span></span>|<span data-ttu-id="3307a-137">String</span><span class="sxs-lookup"><span data-stu-id="3307a-137">String</span></span>|<span data-ttu-id="3307a-138">Apple ID は、現在のトークンを取得するために使用します。</span><span class="sxs-lookup"><span data-stu-id="3307a-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="3307a-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3307a-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="3307a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3307a-140">DateTimeOffset</span></span>|<span data-ttu-id="3307a-141">トークンの期限が切れる。</span><span class="sxs-lookup"><span data-stu-id="3307a-141">When the token will expire.</span></span>|
|<span data-ttu-id="3307a-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3307a-142">lastModifiedDateTime</span></span>|<span data-ttu-id="3307a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3307a-143">DateTimeOffset</span></span>|<span data-ttu-id="3307a-144">Onboarded でした。</span><span class="sxs-lookup"><span data-stu-id="3307a-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="3307a-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3307a-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="3307a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3307a-146">DateTimeOffset</span></span>|<span data-ttu-id="3307a-147">Intune のサービスの最後の syned</span><span class="sxs-lookup"><span data-stu-id="3307a-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="3307a-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="3307a-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="3307a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3307a-149">DateTimeOffset</span></span>|<span data-ttu-id="3307a-150">Intune が最後に同期を要求された場合。</span><span class="sxs-lookup"><span data-stu-id="3307a-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="3307a-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="3307a-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="3307a-152">ブール型</span><span class="sxs-lookup"><span data-stu-id="3307a-152">Boolean</span></span>|<span data-ttu-id="3307a-153">かどうか Dep トークンの共有は学校のデータ同期サービスで有効になります。</span><span class="sxs-lookup"><span data-stu-id="3307a-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="3307a-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="3307a-154">lastSyncErrorCode</span></span>|<span data-ttu-id="3307a-155">Int32</span><span class="sxs-lookup"><span data-stu-id="3307a-155">Int32</span></span>|<span data-ttu-id="3307a-156">Dep の前回の同期中に、Apple によって報告されたエラー ・ コードです。</span><span class="sxs-lookup"><span data-stu-id="3307a-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="3307a-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="3307a-157">tokenType</span></span>|[<span data-ttu-id="3307a-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="3307a-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="3307a-159">Dep のトークンの種類を設定を取得または取得します。</span><span class="sxs-lookup"><span data-stu-id="3307a-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="3307a-160">可能な値は、`none`、`dep`、`appleSchoolManager` です。</span><span class="sxs-lookup"><span data-stu-id="3307a-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="3307a-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="3307a-161">tokenName</span></span>|<span data-ttu-id="3307a-162">String</span><span class="sxs-lookup"><span data-stu-id="3307a-162">String</span></span>|<span data-ttu-id="3307a-163">Dep のトークンの表示名</span><span class="sxs-lookup"><span data-stu-id="3307a-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="3307a-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3307a-164">syncedDeviceCount</span></span>|<span data-ttu-id="3307a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3307a-165">Int32</span></span>|<span data-ttu-id="3307a-166">同期されたデバイスの数を取得</span><span class="sxs-lookup"><span data-stu-id="3307a-166">Gets synced device count</span></span>|
|<span data-ttu-id="3307a-167">defaultProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="3307a-167">defaultProfileDisplayName</span></span>|<span data-ttu-id="3307a-168">String</span><span class="sxs-lookup"><span data-stu-id="3307a-168">String</span></span>|<span data-ttu-id="3307a-169">同期されたデバイスの数を取得</span><span class="sxs-lookup"><span data-stu-id="3307a-169">Gets synced device count</span></span>|
|<span data-ttu-id="3307a-170">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="3307a-170">dataSharingConsentGranted</span></span>|<span data-ttu-id="3307a-171">ブール型</span><span class="sxs-lookup"><span data-stu-id="3307a-171">Boolean</span></span>|<span data-ttu-id="3307a-172">アップル Dep のサービスと共有データの許可に同意するもの</span><span class="sxs-lookup"><span data-stu-id="3307a-172">Consent granted for data sharing with Apple Dep Service</span></span>|



## <a name="response"></a><span data-ttu-id="3307a-173">応答</span><span class="sxs-lookup"><span data-stu-id="3307a-173">Response</span></span>
<span data-ttu-id="3307a-174">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3307a-174">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3307a-175">例</span><span class="sxs-lookup"><span data-stu-id="3307a-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="3307a-176">要求</span><span class="sxs-lookup"><span data-stu-id="3307a-176">Request</span></span>
<span data-ttu-id="3307a-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3307a-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
Content-type: application/json
Content-length: 648

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
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
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```

### <a name="response"></a><span data-ttu-id="3307a-178">応答</span><span class="sxs-lookup"><span data-stu-id="3307a-178">Response</span></span>
<span data-ttu-id="3307a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3307a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 697

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
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```




