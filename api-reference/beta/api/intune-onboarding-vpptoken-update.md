---
title: VPPトークンの更新
description: VPPトークン オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c7e21c740212540ab9d8b76431da4e85312051d5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352246"
---
# <a name="update-vpptoken"></a><span data-ttu-id="f9d00-103">VPPトークンの更新</span><span class="sxs-lookup"><span data-stu-id="f9d00-103">Update vppToken</span></span>

> <span data-ttu-id="f9d00-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9d00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9d00-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9d00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9d00-106">[VPPトークン](../resources/intune-onboarding-vpptoken.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f9d00-106">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9d00-107">必要条件</span><span class="sxs-lookup"><span data-stu-id="f9d00-107">Prerequisites</span></span>
<span data-ttu-id="f9d00-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9d00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9d00-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f9d00-110">Permission type</span></span>|<span data-ttu-id="f9d00-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f9d00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9d00-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f9d00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9d00-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9d00-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f9d00-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9d00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9d00-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9d00-115">Not supported.</span></span>|
|<span data-ttu-id="f9d00-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f9d00-116">Application</span></span>|<span data-ttu-id="f9d00-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9d00-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9d00-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9d00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="f9d00-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9d00-119">Request headers</span></span>
|<span data-ttu-id="f9d00-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9d00-120">Header</span></span>|<span data-ttu-id="f9d00-121">値</span><span class="sxs-lookup"><span data-stu-id="f9d00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9d00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9d00-122">Authorization</span></span>|<span data-ttu-id="f9d00-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9d00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9d00-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f9d00-124">Accept</span></span>|<span data-ttu-id="f9d00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9d00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9d00-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f9d00-126">Request body</span></span>
<span data-ttu-id="f9d00-127">要求本文で、[VPPトークン](../resources/intune-onboarding-vpptoken.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9d00-127">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="f9d00-128">次の表に、[VPPトークン](../resources/intune-onboarding-vpptoken.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f9d00-128">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="f9d00-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9d00-129">Property</span></span>|<span data-ttu-id="f9d00-130">型</span><span class="sxs-lookup"><span data-stu-id="f9d00-130">Type</span></span>|<span data-ttu-id="f9d00-131">説明</span><span class="sxs-lookup"><span data-stu-id="f9d00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9d00-132">id</span><span class="sxs-lookup"><span data-stu-id="f9d00-132">id</span></span>|<span data-ttu-id="f9d00-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f9d00-133">String</span></span>|<span data-ttu-id="f9d00-134">appleVolumePurchaseProgramToken 作成時に自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="f9d00-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="f9d00-135">エンティティのキーになります。</span><span class="sxs-lookup"><span data-stu-id="f9d00-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="f9d00-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="f9d00-136">organizationName</span></span>|<span data-ttu-id="f9d00-137">String</span><span class="sxs-lookup"><span data-stu-id="f9d00-137">String</span></span>|<span data-ttu-id="f9d00-138">Apple ボリューム購入プログラムのトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="f9d00-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="f9d00-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="f9d00-139">vppTokenAccountType</span></span>|[<span data-ttu-id="f9d00-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="f9d00-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="f9d00-141">特定の Apple ボリューム購入プログラムのトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="f9d00-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="f9d00-142">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="f9d00-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="f9d00-143">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="f9d00-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="f9d00-144">appleId</span><span class="sxs-lookup"><span data-stu-id="f9d00-144">appleId</span></span>|<span data-ttu-id="f9d00-145">String</span><span class="sxs-lookup"><span data-stu-id="f9d00-145">String</span></span>|<span data-ttu-id="f9d00-146">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="f9d00-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f9d00-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f9d00-147">expirationDateTime</span></span>|<span data-ttu-id="f9d00-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9d00-148">DateTimeOffset</span></span>|<span data-ttu-id="f9d00-149">Apple ボリューム購入プログラムのトークンの有効期限。</span><span class="sxs-lookup"><span data-stu-id="f9d00-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f9d00-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f9d00-150">lastSyncDateTime</span></span>|<span data-ttu-id="f9d00-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9d00-151">DateTimeOffset</span></span>|<span data-ttu-id="f9d00-152">Apple ボリューム購入プログラムのトークンを使用して、Apple ボリューム購入プログラム サービスと最後にアプリケーションの同期を行った日時。</span><span class="sxs-lookup"><span data-stu-id="f9d00-152">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f9d00-153">token</span><span class="sxs-lookup"><span data-stu-id="f9d00-153">token</span></span>|<span data-ttu-id="f9d00-154">String</span><span class="sxs-lookup"><span data-stu-id="f9d00-154">String</span></span>|<span data-ttu-id="f9d00-155">Apple ボリューム購入プログラムからダウンロードした Apple ボリューム購入プログラムのトークン文字列。</span><span class="sxs-lookup"><span data-stu-id="f9d00-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="f9d00-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9d00-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f9d00-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9d00-157">DateTimeOffset</span></span>|<span data-ttu-id="f9d00-158">Apple ボリューム購入プログラムのトークンに関連付けられている最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="f9d00-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f9d00-159">state</span><span class="sxs-lookup"><span data-stu-id="f9d00-159">state</span></span>|[<span data-ttu-id="f9d00-160">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="f9d00-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="f9d00-161">Apple ボリューム購入プログラムのトークンの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="f9d00-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="f9d00-162">可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。</span><span class="sxs-lookup"><span data-stu-id="f9d00-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="f9d00-163">可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。</span><span class="sxs-lookup"><span data-stu-id="f9d00-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="f9d00-164">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="f9d00-164">tokenActionResults</span></span>|<span data-ttu-id="f9d00-165">[Vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f9d00-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="f9d00-166">Apple Volume Purchase Program トークンで実行されたアクションのステータスのコレクション。</span><span class="sxs-lookup"><span data-stu-id="f9d00-166">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f9d00-167">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="f9d00-167">lastSyncStatus</span></span>|[<span data-ttu-id="f9d00-168">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="f9d00-168">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="f9d00-169">Apple ボリューム購入プログラム トークンを使用して行われた最後のアプリケーションの同期の現在の同期状態。</span><span class="sxs-lookup"><span data-stu-id="f9d00-169">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="f9d00-170">可能な値は、`none`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="f9d00-170">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="f9d00-171">可能な値は、`none`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="f9d00-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="f9d00-172">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="f9d00-172">automaticallyUpdateApps</span></span>|<span data-ttu-id="f9d00-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9d00-173">Boolean</span></span>|<span data-ttu-id="f9d00-174">VPP トークンのアプリを自動で更新するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f9d00-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="f9d00-175">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="f9d00-175">countryOrRegion</span></span>|<span data-ttu-id="f9d00-176">文字列</span><span class="sxs-lookup"><span data-stu-id="f9d00-176">String</span></span>|<span data-ttu-id="f9d00-177">VPP トークンのアプリを自動で更新するかどうか。</span><span class="sxs-lookup"><span data-stu-id="f9d00-177">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="f9d00-178">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="f9d00-178">dataSharingConsentGranted</span></span>|<span data-ttu-id="f9d00-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9d00-179">Boolean</span></span>|<span data-ttu-id="f9d00-180">Apple Volume Purchase Program でのデータ共有に対して付与される同意。</span><span class="sxs-lookup"><span data-stu-id="f9d00-180">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="f9d00-181">displayName</span><span class="sxs-lookup"><span data-stu-id="f9d00-181">displayName</span></span>|<span data-ttu-id="f9d00-182">String</span><span class="sxs-lookup"><span data-stu-id="f9d00-182">String</span></span>|<span data-ttu-id="f9d00-183">管理者が指定したトークンのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="f9d00-183">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="f9d00-184">Msrtcsip-locationname</span><span class="sxs-lookup"><span data-stu-id="f9d00-184">locationName</span></span>|<span data-ttu-id="f9d00-185">String</span><span class="sxs-lookup"><span data-stu-id="f9d00-185">String</span></span>|<span data-ttu-id="f9d00-186">Apple VPP から返されるトークンの場所。</span><span class="sxs-lookup"><span data-stu-id="f9d00-186">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="f9d00-187">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="f9d00-187">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="f9d00-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9d00-188">Boolean</span></span>|<span data-ttu-id="f9d00-189">管理者の同意を得て、外部 MDM からのトークン管理を許可します。</span><span class="sxs-lookup"><span data-stu-id="f9d00-189">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="f9d00-190">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f9d00-190">roleScopeTagIds</span></span>|<span data-ttu-id="f9d00-191">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f9d00-191">String collection</span></span>|<span data-ttu-id="f9d00-192">このエンティティに割り当てられているロールスコープタグ Id。</span><span class="sxs-lookup"><span data-stu-id="f9d00-192">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="f9d00-193">応答</span><span class="sxs-lookup"><span data-stu-id="f9d00-193">Response</span></span>
<span data-ttu-id="f9d00-194">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [VPPトークン](../resources/intune-onboarding-vpptoken.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f9d00-194">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9d00-195">例</span><span class="sxs-lookup"><span data-stu-id="f9d00-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9d00-196">要求</span><span class="sxs-lookup"><span data-stu-id="f9d00-196">Request</span></span>
<span data-ttu-id="f9d00-197">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f9d00-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 1002

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
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
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="f9d00-198">応答</span><span class="sxs-lookup"><span data-stu-id="f9d00-198">Response</span></span>
<span data-ttu-id="f9d00-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f9d00-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1115

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
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```






