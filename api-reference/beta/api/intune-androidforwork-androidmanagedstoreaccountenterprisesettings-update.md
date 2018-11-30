---
title: AndroidManagedStoreAccountEnterpriseSettings を更新します。
description: AndroidManagedStoreAccountEnterpriseSettings オブジェクトのプロパティを更新します。
ms.openlocfilehash: 383c9225076e9e68e9b34d89b7fe904ccf747224
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069587"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="fcce1-103">AndroidManagedStoreAccountEnterpriseSettings を更新します。</span><span class="sxs-lookup"><span data-stu-id="fcce1-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="fcce1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fcce1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcce1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fcce1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fcce1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fcce1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcce1-107">[AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fcce1-107">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fcce1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fcce1-108">Prerequisites</span></span>
<span data-ttu-id="fcce1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fcce1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcce1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fcce1-111">Permission type</span></span>|<span data-ttu-id="fcce1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fcce1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcce1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fcce1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fcce1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcce1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fcce1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fcce1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcce1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fcce1-116">Not supported.</span></span>|
|<span data-ttu-id="fcce1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fcce1-117">Application</span></span>|<span data-ttu-id="fcce1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fcce1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcce1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fcce1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="fcce1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fcce1-120">Request headers</span></span>
|<span data-ttu-id="fcce1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fcce1-121">Header</span></span>|<span data-ttu-id="fcce1-122">値</span><span class="sxs-lookup"><span data-stu-id="fcce1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcce1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcce1-123">Authorization</span></span>|<span data-ttu-id="fcce1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fcce1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcce1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fcce1-125">Accept</span></span>|<span data-ttu-id="fcce1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fcce1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcce1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fcce1-127">Request body</span></span>
<span data-ttu-id="fcce1-128">要求の本文に[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="fcce1-128">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="fcce1-129">[AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="fcce1-129">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="fcce1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fcce1-130">Property</span></span>|<span data-ttu-id="fcce1-131">型</span><span class="sxs-lookup"><span data-stu-id="fcce1-131">Type</span></span>|<span data-ttu-id="fcce1-132">説明</span><span class="sxs-lookup"><span data-stu-id="fcce1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcce1-133">id</span><span class="sxs-lookup"><span data-stu-id="fcce1-133">id</span></span>|<span data-ttu-id="fcce1-134">String</span><span class="sxs-lookup"><span data-stu-id="fcce1-134">String</span></span>|<span data-ttu-id="fcce1-135">アカウントのエンタープライズ設定の識別子を格納する、アプリ</span><span class="sxs-lookup"><span data-stu-id="fcce1-135">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="fcce1-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="fcce1-136">bindStatus</span></span>|[<span data-ttu-id="fcce1-137">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="fcce1-137">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="fcce1-138">Google の EMM の API を使用してテナントの状態をバインドします。</span><span class="sxs-lookup"><span data-stu-id="fcce1-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="fcce1-139">可能な値は、`notBound`、`bound`、`boundAndValidated`、`unbinding` です。</span><span class="sxs-lookup"><span data-stu-id="fcce1-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="fcce1-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fcce1-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="fcce1-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcce1-141">DateTimeOffset</span></span>|<span data-ttu-id="fcce1-142">アプリ同期の最終完了時刻</span><span class="sxs-lookup"><span data-stu-id="fcce1-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="fcce1-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="fcce1-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="fcce1-144">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="fcce1-144">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="fcce1-145">アプリケーション同期の最終結果です。</span><span class="sxs-lookup"><span data-stu-id="fcce1-145">Last application sync result.</span></span> <span data-ttu-id="fcce1-146">使用可能な値: `success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="fcce1-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="fcce1-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fcce1-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="fcce1-148">String</span><span class="sxs-lookup"><span data-stu-id="fcce1-148">String</span></span>|<span data-ttu-id="fcce1-149">エンタープライズを作成した所有者 UPN</span><span class="sxs-lookup"><span data-stu-id="fcce1-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="fcce1-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="fcce1-150">ownerOrganizationName</span></span>|<span data-ttu-id="fcce1-151">String</span><span class="sxs-lookup"><span data-stu-id="fcce1-151">String</span></span>|<span data-ttu-id="fcce1-152">組織名を使用する場合 Android のエンタープライズ契約時</span><span class="sxs-lookup"><span data-stu-id="fcce1-152">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="fcce1-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fcce1-153">lastModifiedDateTime</span></span>|<span data-ttu-id="fcce1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcce1-154">DateTimeOffset</span></span>|<span data-ttu-id="fcce1-155">Android エンタープライズ設定の最終変更時刻</span><span class="sxs-lookup"><span data-stu-id="fcce1-155">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="fcce1-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="fcce1-156">enrollmentTarget</span></span>|[<span data-ttu-id="fcce1-157">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="fcce1-157">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="fcce1-158">Android エンタープライズ デバイスの管理デバイスを登録できるユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="fcce1-158">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="fcce1-159">可能な値は、`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="fcce1-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="fcce1-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="fcce1-160">targetGroupIds</span></span>|<span data-ttu-id="fcce1-161">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fcce1-161">String collection</span></span>|<span data-ttu-id="fcce1-162">enrollmentTarget が 'Targeted' に設定されている場合、どの AAD グループが Android for Work デバイス管理にデバイスを登録できるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="fcce1-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="fcce1-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="fcce1-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="fcce1-164">ブール値</span><span class="sxs-lookup"><span data-stu-id="fcce1-164">Boolean</span></span>|<span data-ttu-id="fcce1-165">このアカウントを CloudDPC に Android のデバイスの所有者の管理の flighting かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fcce1-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="fcce1-166">応答</span><span class="sxs-lookup"><span data-stu-id="fcce1-166">Response</span></span>
<span data-ttu-id="fcce1-167">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="fcce1-167">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcce1-168">例</span><span class="sxs-lookup"><span data-stu-id="fcce1-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="fcce1-169">要求</span><span class="sxs-lookup"><span data-stu-id="fcce1-169">Request</span></span>
<span data-ttu-id="fcce1-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fcce1-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
Content-type: application/json
Content-length: 458

{
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="fcce1-171">応答</span><span class="sxs-lookup"><span data-stu-id="fcce1-171">Response</span></span>
<span data-ttu-id="fcce1-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fcce1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "id": "b71357c9-57c9-b713-c957-13b7c95713b7",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```





