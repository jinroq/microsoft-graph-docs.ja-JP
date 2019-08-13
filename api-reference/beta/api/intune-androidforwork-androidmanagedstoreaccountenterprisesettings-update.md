---
title: AndroidManagedStoreAccountEnterpriseSettings の更新
description: AndroidManagedStoreAccountEnterpriseSettings オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b517e2db80bf3e580a21d5117f7a279144e96c1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324967"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="10e0f-103">AndroidManagedStoreAccountEnterpriseSettings の更新</span><span class="sxs-lookup"><span data-stu-id="10e0f-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="10e0f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10e0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10e0f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="10e0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10e0f-106">[Androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="10e0f-106">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10e0f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="10e0f-107">Prerequisites</span></span>
<span data-ttu-id="10e0f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="10e0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10e0f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="10e0f-110">Permission type</span></span>|<span data-ttu-id="10e0f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="10e0f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10e0f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="10e0f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10e0f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10e0f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="10e0f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="10e0f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10e0f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10e0f-115">Not supported.</span></span>|
|<span data-ttu-id="10e0f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="10e0f-116">Application</span></span>|<span data-ttu-id="10e0f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10e0f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10e0f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="10e0f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="10e0f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="10e0f-119">Request headers</span></span>
|<span data-ttu-id="10e0f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="10e0f-120">Header</span></span>|<span data-ttu-id="10e0f-121">値</span><span class="sxs-lookup"><span data-stu-id="10e0f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10e0f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="10e0f-122">Authorization</span></span>|<span data-ttu-id="10e0f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="10e0f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10e0f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="10e0f-124">Accept</span></span>|<span data-ttu-id="10e0f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10e0f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10e0f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="10e0f-126">Request body</span></span>
<span data-ttu-id="10e0f-127">要求本文で、 [Androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="10e0f-127">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="10e0f-128">次の表に、 [Androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="10e0f-128">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="10e0f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10e0f-129">Property</span></span>|<span data-ttu-id="10e0f-130">型</span><span class="sxs-lookup"><span data-stu-id="10e0f-130">Type</span></span>|<span data-ttu-id="10e0f-131">説明</span><span class="sxs-lookup"><span data-stu-id="10e0f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10e0f-132">id</span><span class="sxs-lookup"><span data-stu-id="10e0f-132">id</span></span>|<span data-ttu-id="10e0f-133">String</span><span class="sxs-lookup"><span data-stu-id="10e0f-133">String</span></span>|<span data-ttu-id="10e0f-134">Android ストアアカウントのエンタープライズ設定識別子</span><span class="sxs-lookup"><span data-stu-id="10e0f-134">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="10e0f-135">bindStatus</span><span class="sxs-lookup"><span data-stu-id="10e0f-135">bindStatus</span></span>|[<span data-ttu-id="10e0f-136">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="10e0f-136">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="10e0f-137">Google EMM API を使用して、テナントの状態をバインドします。</span><span class="sxs-lookup"><span data-stu-id="10e0f-137">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="10e0f-138">使用可能な値は、`notBound`、`bound`、`boundAndValidated`、`unbinding` です。</span><span class="sxs-lookup"><span data-stu-id="10e0f-138">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="10e0f-139">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="10e0f-139">lastAppSyncDateTime</span></span>|<span data-ttu-id="10e0f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10e0f-140">DateTimeOffset</span></span>|<span data-ttu-id="10e0f-141">アプリ同期の最終完了時刻</span><span class="sxs-lookup"><span data-stu-id="10e0f-141">Last completion time for app sync</span></span>|
|<span data-ttu-id="10e0f-142">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="10e0f-142">lastAppSyncStatus</span></span>|[<span data-ttu-id="10e0f-143">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="10e0f-143">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="10e0f-144">最後のアプリケーションの同期結果。</span><span class="sxs-lookup"><span data-stu-id="10e0f-144">Last application sync result.</span></span> <span data-ttu-id="10e0f-145">使用可能な値: `success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="10e0f-145">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="10e0f-146">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="10e0f-146">ownerUserPrincipalName</span></span>|<span data-ttu-id="10e0f-147">String</span><span class="sxs-lookup"><span data-stu-id="10e0f-147">String</span></span>|<span data-ttu-id="10e0f-148">エンタープライズを作成した所有者の UPN</span><span class="sxs-lookup"><span data-stu-id="10e0f-148">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="10e0f-149">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="10e0f-149">ownerOrganizationName</span></span>|<span data-ttu-id="10e0f-150">String</span><span class="sxs-lookup"><span data-stu-id="10e0f-150">String</span></span>|<span data-ttu-id="10e0f-151">Android Enterprise のオンボード時に使用される組織名</span><span class="sxs-lookup"><span data-stu-id="10e0f-151">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="10e0f-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10e0f-152">lastModifiedDateTime</span></span>|<span data-ttu-id="10e0f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10e0f-153">DateTimeOffset</span></span>|<span data-ttu-id="10e0f-154">Android エンタープライズ設定の最終変更時刻</span><span class="sxs-lookup"><span data-stu-id="10e0f-154">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="10e0f-155">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="10e0f-155">enrollmentTarget</span></span>|[<span data-ttu-id="10e0f-156">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="10e0f-156">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="10e0f-157">Android エンタープライズデバイス管理にデバイスを登録できるユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="10e0f-157">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="10e0f-158">使用可能な値は、`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="10e0f-158">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="10e0f-159">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="10e0f-159">targetGroupIds</span></span>|<span data-ttu-id="10e0f-160">String コレクション</span><span class="sxs-lookup"><span data-stu-id="10e0f-160">String collection</span></span>|<span data-ttu-id="10e0f-161">enrollmentTarget が「Targeted」に設定されている場合、どの AAD グループが Android for Work デバイス管理にデバイスを登録できるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="10e0f-161">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="10e0f-162">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="10e0f-162">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="10e0f-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="10e0f-163">Boolean</span></span>|<span data-ttu-id="10e0f-164">CloudDPC を使用した Android デバイス所有者の管理に、このアカウントが flighting になるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="10e0f-164">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|
|<span data-ttu-id="10e0f-165">会社コード</span><span class="sxs-lookup"><span data-stu-id="10e0f-165">companyCodes</span></span>|<span data-ttu-id="10e0f-166">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="10e0f-166">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) collection</span></span>|<span data-ttu-id="10e0f-167">AndroidManagedStoreAccountEnterpriseSettings の会社コード</span><span class="sxs-lookup"><span data-stu-id="10e0f-167">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|
|<span data-ttu-id="10e0f-168">androidDeviceOwnerFullyManagedEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="10e0f-168">androidDeviceOwnerFullyManagedEnrollmentEnabled</span></span>|<span data-ttu-id="10e0f-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="10e0f-169">Boolean</span></span>|<span data-ttu-id="10e0f-170">AndroidManagedStoreAccountEnterpriseSettings の会社コード</span><span class="sxs-lookup"><span data-stu-id="10e0f-170">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|



## <a name="response"></a><span data-ttu-id="10e0f-171">応答</span><span class="sxs-lookup"><span data-stu-id="10e0f-171">Response</span></span>
<span data-ttu-id="10e0f-172">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="10e0f-172">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10e0f-173">例</span><span class="sxs-lookup"><span data-stu-id="10e0f-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="10e0f-174">要求</span><span class="sxs-lookup"><span data-stu-id="10e0f-174">Request</span></span>
<span data-ttu-id="10e0f-175">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="10e0f-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
Content-type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "Enrollment Token value",
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="10e0f-176">応答</span><span class="sxs-lookup"><span data-stu-id="10e0f-176">Response</span></span>
<span data-ttu-id="10e0f-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="10e0f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1010

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
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "Enrollment Token value",
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```






