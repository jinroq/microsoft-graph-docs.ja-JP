---
title: VPPトークンの更新
description: vppToken オブジェクトのプロパティを更新します。
ms.openlocfilehash: 2fdcb0d78b0690b63df429f43976647e93e6f25c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066856"
---
# <a name="update-vpptoken"></a><span data-ttu-id="f078a-103">VPPトークンの更新</span><span class="sxs-lookup"><span data-stu-id="f078a-103">Update vppToken</span></span>

> <span data-ttu-id="f078a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f078a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f078a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f078a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f078a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f078a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f078a-107">[VPPトークン](../resources/intune-onboarding-vpptoken.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f078a-107">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f078a-108">必要条件</span><span class="sxs-lookup"><span data-stu-id="f078a-108">Prerequisites</span></span>
<span data-ttu-id="f078a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f078a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f078a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f078a-111">Permission type</span></span>|<span data-ttu-id="f078a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f078a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f078a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f078a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f078a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f078a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f078a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f078a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f078a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f078a-116">Not supported.</span></span>|
|<span data-ttu-id="f078a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f078a-117">Application</span></span>|<span data-ttu-id="f078a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f078a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f078a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f078a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="f078a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f078a-120">Request headers</span></span>
|<span data-ttu-id="f078a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f078a-121">Header</span></span>|<span data-ttu-id="f078a-122">値</span><span class="sxs-lookup"><span data-stu-id="f078a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f078a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f078a-123">Authorization</span></span>|<span data-ttu-id="f078a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f078a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f078a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f078a-125">Accept</span></span>|<span data-ttu-id="f078a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f078a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f078a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f078a-127">Request body</span></span>
<span data-ttu-id="f078a-128">要求本文で、[VPPトークン](../resources/intune-onboarding-vpptoken.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f078a-128">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="f078a-129">次の表に、[VPPトークン](../resources/intune-onboarding-vpptoken.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f078a-129">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="f078a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f078a-130">Property</span></span>|<span data-ttu-id="f078a-131">型</span><span class="sxs-lookup"><span data-stu-id="f078a-131">Type</span></span>|<span data-ttu-id="f078a-132">説明</span><span class="sxs-lookup"><span data-stu-id="f078a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f078a-133">id</span><span class="sxs-lookup"><span data-stu-id="f078a-133">id</span></span>|<span data-ttu-id="f078a-134">String</span><span class="sxs-lookup"><span data-stu-id="f078a-134">String</span></span>|<span data-ttu-id="f078a-135">appleVolumePurchaseProgramToken 作成時に自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="f078a-135">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="f078a-136">エンティティのキーになります。</span><span class="sxs-lookup"><span data-stu-id="f078a-136">It is the Key of the entity.</span></span>|
|<span data-ttu-id="f078a-137">organizationName</span><span class="sxs-lookup"><span data-stu-id="f078a-137">organizationName</span></span>|<span data-ttu-id="f078a-138">String</span><span class="sxs-lookup"><span data-stu-id="f078a-138">String</span></span>|<span data-ttu-id="f078a-139">Apple Volume Purchase Program のトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="f078a-139">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="f078a-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="f078a-140">vppTokenAccountType</span></span>|[<span data-ttu-id="f078a-141">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="f078a-141">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="f078a-142">特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="f078a-142">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="f078a-143">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="f078a-143">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="f078a-144">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="f078a-144">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="f078a-145">appleId</span><span class="sxs-lookup"><span data-stu-id="f078a-145">appleId</span></span>|<span data-ttu-id="f078a-146">String</span><span class="sxs-lookup"><span data-stu-id="f078a-146">String</span></span>|<span data-ttu-id="f078a-147">特定の Apple Volume Purchase Program のトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="f078a-147">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f078a-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f078a-148">expirationDateTime</span></span>|<span data-ttu-id="f078a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f078a-149">DateTimeOffset</span></span>|<span data-ttu-id="f078a-150">Apple Volume Purchase Program のトークンの有効期限。</span><span class="sxs-lookup"><span data-stu-id="f078a-150">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f078a-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f078a-151">lastSyncDateTime</span></span>|<span data-ttu-id="f078a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f078a-152">DateTimeOffset</span></span>|<span data-ttu-id="f078a-153">Apple Volume Purchase Program のトークンを使用して、Apple ボリューム購入プログラム サービスと最後にアプリケーションの同期を行った日時。</span><span class="sxs-lookup"><span data-stu-id="f078a-153">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f078a-154">token</span><span class="sxs-lookup"><span data-stu-id="f078a-154">token</span></span>|<span data-ttu-id="f078a-155">String</span><span class="sxs-lookup"><span data-stu-id="f078a-155">String</span></span>|<span data-ttu-id="f078a-156">Apple Volume Purchase Program からダウンロードした Apple ボリューム購入プログラムのトークン文字列。</span><span class="sxs-lookup"><span data-stu-id="f078a-156">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="f078a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f078a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f078a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f078a-158">DateTimeOffset</span></span>|<span data-ttu-id="f078a-159">Apple Volume Purchase Program のトークンに関連付けられている最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="f078a-159">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f078a-160">state</span><span class="sxs-lookup"><span data-stu-id="f078a-160">state</span></span>|[<span data-ttu-id="f078a-161">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="f078a-161">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="f078a-162">Apple Volume Purchase Program のトークンの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="f078a-162">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="f078a-163">可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。</span><span class="sxs-lookup"><span data-stu-id="f078a-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="f078a-164">可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。</span><span class="sxs-lookup"><span data-stu-id="f078a-164">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="f078a-165">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="f078a-165">tokenActionResults</span></span>|<span data-ttu-id="f078a-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f078a-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="f078a-167">アクションの状態のコレクションは、Apple ボリューム購入プログラム トークンで実行されます。</span><span class="sxs-lookup"><span data-stu-id="f078a-167">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f078a-168">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="f078a-168">lastSyncStatus</span></span>|[<span data-ttu-id="f078a-169">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="f078a-169">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="f078a-170">Apple Volume Purchase Program のトークンを使用して行われた最後のアプリケーションの同期の現在の同期状態。</span><span class="sxs-lookup"><span data-stu-id="f078a-170">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="f078a-171">可能な値は、`none`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="f078a-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="f078a-172">可能な値は、`none`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="f078a-172">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="f078a-173">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="f078a-173">automaticallyUpdateApps</span></span>|<span data-ttu-id="f078a-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="f078a-174">Boolean</span></span>|<span data-ttu-id="f078a-175">VPP トークンのアプリを自動で更新するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f078a-175">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="f078a-176">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="f078a-176">countryOrRegion</span></span>|<span data-ttu-id="f078a-177">String</span><span class="sxs-lookup"><span data-stu-id="f078a-177">String</span></span>|<span data-ttu-id="f078a-178">VPP トークンのアプリを自動で更新するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f078a-178">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="f078a-179">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="f078a-179">dataSharingConsentGranted</span></span>|<span data-ttu-id="f078a-180">ブール値</span><span class="sxs-lookup"><span data-stu-id="f078a-180">Boolean</span></span>|<span data-ttu-id="f078a-181">Apple ボリューム購入プログラムを使用して共有データに確かに同意するものです。</span><span class="sxs-lookup"><span data-stu-id="f078a-181">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="f078a-182">displayName</span><span class="sxs-lookup"><span data-stu-id="f078a-182">displayName</span></span>|<span data-ttu-id="f078a-183">String</span><span class="sxs-lookup"><span data-stu-id="f078a-183">String</span></span>|<span data-ttu-id="f078a-184">管理者は、トークンのフレンドリ名を指定します。</span><span class="sxs-lookup"><span data-stu-id="f078a-184">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="f078a-185">locationName</span><span class="sxs-lookup"><span data-stu-id="f078a-185">locationName</span></span>|<span data-ttu-id="f078a-186">String</span><span class="sxs-lookup"><span data-stu-id="f078a-186">String</span></span>|<span data-ttu-id="f078a-187">アップル VPP から返されるトークンの場所です。</span><span class="sxs-lookup"><span data-stu-id="f078a-187">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="f078a-188">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="f078a-188">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="f078a-189">ブール値</span><span class="sxs-lookup"><span data-stu-id="f078a-189">Boolean</span></span>|<span data-ttu-id="f078a-190">外部 MDM. からのトークンの管理であると主張できるようにするのには同意するものと管理</span><span class="sxs-lookup"><span data-stu-id="f078a-190">Admin consent to allow claiming token management from external MDM.</span></span>|



## <a name="response"></a><span data-ttu-id="f078a-191">応答</span><span class="sxs-lookup"><span data-stu-id="f078a-191">Response</span></span>
<span data-ttu-id="f078a-192">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [VPPトークン](../resources/intune-onboarding-vpptoken.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f078a-192">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f078a-193">例</span><span class="sxs-lookup"><span data-stu-id="f078a-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="f078a-194">要求</span><span class="sxs-lookup"><span data-stu-id="f078a-194">Request</span></span>
<span data-ttu-id="f078a-195">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f078a-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 957

{
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true
}
```

### <a name="response"></a><span data-ttu-id="f078a-196">応答</span><span class="sxs-lookup"><span data-stu-id="f078a-196">Response</span></span>
<span data-ttu-id="f078a-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f078a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1053

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true
}
```





