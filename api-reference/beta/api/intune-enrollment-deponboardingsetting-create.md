---
title: DepOnboardingSetting を作成します。
description: 新しい depOnboardingSetting オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6aa17e5741df007d7ee449a4ab305be37807051d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409819"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="b1f47-103">DepOnboardingSetting を作成します。</span><span class="sxs-lookup"><span data-stu-id="b1f47-103">Create depOnboardingSetting</span></span>

> <span data-ttu-id="b1f47-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b1f47-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b1f47-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1f47-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1f47-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b1f47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1f47-107">新しい[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b1f47-107">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1f47-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b1f47-108">Prerequisites</span></span>
<span data-ttu-id="b1f47-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1f47-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b1f47-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1f47-111">Permission type</span></span>|<span data-ttu-id="b1f47-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1f47-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1f47-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1f47-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1f47-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1f47-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b1f47-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1f47-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1f47-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1f47-116">Not supported.</span></span>|
|<span data-ttu-id="b1f47-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1f47-117">Application</span></span>|<span data-ttu-id="b1f47-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1f47-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1f47-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1f47-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="b1f47-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1f47-120">Request headers</span></span>
|<span data-ttu-id="b1f47-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1f47-121">Header</span></span>|<span data-ttu-id="b1f47-122">値</span><span class="sxs-lookup"><span data-stu-id="b1f47-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1f47-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1f47-123">Authorization</span></span>|<span data-ttu-id="b1f47-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b1f47-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1f47-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1f47-125">Accept</span></span>|<span data-ttu-id="b1f47-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1f47-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1f47-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1f47-127">Request body</span></span>
<span data-ttu-id="b1f47-128">要求の本文に depOnboardingSetting オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b1f47-128">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="b1f47-129">次の表は、depOnboardingSetting を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b1f47-129">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="b1f47-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1f47-130">Property</span></span>|<span data-ttu-id="b1f47-131">型</span><span class="sxs-lookup"><span data-stu-id="b1f47-131">Type</span></span>|<span data-ttu-id="b1f47-132">説明</span><span class="sxs-lookup"><span data-stu-id="b1f47-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1f47-133">id</span><span class="sxs-lookup"><span data-stu-id="b1f47-133">id</span></span>|<span data-ttu-id="b1f47-134">String</span><span class="sxs-lookup"><span data-stu-id="b1f47-134">String</span></span>|<span data-ttu-id="b1f47-135">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="b1f47-135">UUID for the object</span></span>|
|<span data-ttu-id="b1f47-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="b1f47-136">appleIdentifier</span></span>|<span data-ttu-id="b1f47-137">String</span><span class="sxs-lookup"><span data-stu-id="b1f47-137">String</span></span>|<span data-ttu-id="b1f47-138">Apple ID は、現在のトークンを取得するために使用します。</span><span class="sxs-lookup"><span data-stu-id="b1f47-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="b1f47-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b1f47-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="b1f47-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1f47-140">DateTimeOffset</span></span>|<span data-ttu-id="b1f47-141">トークンの期限が切れる。</span><span class="sxs-lookup"><span data-stu-id="b1f47-141">When the token will expire.</span></span>|
|<span data-ttu-id="b1f47-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1f47-142">lastModifiedDateTime</span></span>|<span data-ttu-id="b1f47-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1f47-143">DateTimeOffset</span></span>|<span data-ttu-id="b1f47-144">Onboarded でした。</span><span class="sxs-lookup"><span data-stu-id="b1f47-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="b1f47-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b1f47-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="b1f47-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1f47-146">DateTimeOffset</span></span>|<span data-ttu-id="b1f47-147">Intune のサービスの最後の syned</span><span class="sxs-lookup"><span data-stu-id="b1f47-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="b1f47-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="b1f47-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="b1f47-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1f47-149">DateTimeOffset</span></span>|<span data-ttu-id="b1f47-150">Intune が最後に同期を要求された場合。</span><span class="sxs-lookup"><span data-stu-id="b1f47-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="b1f47-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="b1f47-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="b1f47-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1f47-152">Boolean</span></span>|<span data-ttu-id="b1f47-153">かどうか Dep トークンの共有は学校のデータ同期サービスで有効になります。</span><span class="sxs-lookup"><span data-stu-id="b1f47-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="b1f47-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="b1f47-154">lastSyncErrorCode</span></span>|<span data-ttu-id="b1f47-155">Int32</span><span class="sxs-lookup"><span data-stu-id="b1f47-155">Int32</span></span>|<span data-ttu-id="b1f47-156">Dep の前回の同期中に、Apple によって報告されたエラー ・ コードです。</span><span class="sxs-lookup"><span data-stu-id="b1f47-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="b1f47-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="b1f47-157">tokenType</span></span>|[<span data-ttu-id="b1f47-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="b1f47-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="b1f47-159">Dep のトークンの種類を設定を取得または取得します。</span><span class="sxs-lookup"><span data-stu-id="b1f47-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="b1f47-160">可能な値は、`none`、`dep`、`appleSchoolManager` です。</span><span class="sxs-lookup"><span data-stu-id="b1f47-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="b1f47-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="b1f47-161">tokenName</span></span>|<span data-ttu-id="b1f47-162">String</span><span class="sxs-lookup"><span data-stu-id="b1f47-162">String</span></span>|<span data-ttu-id="b1f47-163">Dep のトークンの表示名</span><span class="sxs-lookup"><span data-stu-id="b1f47-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="b1f47-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1f47-164">syncedDeviceCount</span></span>|<span data-ttu-id="b1f47-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b1f47-165">Int32</span></span>|<span data-ttu-id="b1f47-166">同期されたデバイスの数を取得</span><span class="sxs-lookup"><span data-stu-id="b1f47-166">Gets synced device count</span></span>|
|<span data-ttu-id="b1f47-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="b1f47-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="b1f47-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1f47-168">Boolean</span></span>|<span data-ttu-id="b1f47-169">アップル Dep のサービスと共有データの許可に同意するもの</span><span class="sxs-lookup"><span data-stu-id="b1f47-169">Consent granted for data sharing with Apple Dep Service</span></span>|



## <a name="response"></a><span data-ttu-id="b1f47-170">応答</span><span class="sxs-lookup"><span data-stu-id="b1f47-170">Response</span></span>
<span data-ttu-id="b1f47-171">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b1f47-171">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1f47-172">例</span><span class="sxs-lookup"><span data-stu-id="b1f47-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1f47-173">要求</span><span class="sxs-lookup"><span data-stu-id="b1f47-173">Request</span></span>
<span data-ttu-id="b1f47-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b1f47-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
Content-type: application/json
Content-length: 514

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
  "dataSharingConsentGranted": true
}
```

### <a name="response"></a><span data-ttu-id="b1f47-175">応答</span><span class="sxs-lookup"><span data-stu-id="b1f47-175">Response</span></span>
<span data-ttu-id="b1f47-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b1f47-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 627

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
  "dataSharingConsentGranted": true
}
```




