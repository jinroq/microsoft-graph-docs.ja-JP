---
title: androidmanagedstoreaccountenterprisesettings の更新
description: androidmanagedstoreaccountenterprisesettings オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d7a131c98fa5a175435df01837a674eb4fbe747
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139719"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="74f2e-103">androidmanagedstoreaccountenterprisesettings の更新</span><span class="sxs-lookup"><span data-stu-id="74f2e-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="74f2e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74f2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74f2e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="74f2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74f2e-106">[androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="74f2e-106">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74f2e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="74f2e-107">Prerequisites</span></span>
<span data-ttu-id="74f2e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74f2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="74f2e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74f2e-110">Permission type</span></span>|<span data-ttu-id="74f2e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="74f2e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74f2e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74f2e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74f2e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74f2e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74f2e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74f2e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74f2e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74f2e-115">Not supported.</span></span>|
|<span data-ttu-id="74f2e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74f2e-116">Application</span></span>|<span data-ttu-id="74f2e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74f2e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74f2e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74f2e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="74f2e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74f2e-119">Request headers</span></span>
|<span data-ttu-id="74f2e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74f2e-120">Header</span></span>|<span data-ttu-id="74f2e-121">値</span><span class="sxs-lookup"><span data-stu-id="74f2e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74f2e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="74f2e-122">Authorization</span></span>|<span data-ttu-id="74f2e-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="74f2e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74f2e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="74f2e-124">Accept</span></span>|<span data-ttu-id="74f2e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74f2e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74f2e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="74f2e-126">Request body</span></span>
<span data-ttu-id="74f2e-127">要求本文で、 [androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="74f2e-127">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="74f2e-128">次の表に、 [androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="74f2e-128">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="74f2e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74f2e-129">Property</span></span>|<span data-ttu-id="74f2e-130">型</span><span class="sxs-lookup"><span data-stu-id="74f2e-130">Type</span></span>|<span data-ttu-id="74f2e-131">説明</span><span class="sxs-lookup"><span data-stu-id="74f2e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74f2e-132">id</span><span class="sxs-lookup"><span data-stu-id="74f2e-132">id</span></span>|<span data-ttu-id="74f2e-133">String</span><span class="sxs-lookup"><span data-stu-id="74f2e-133">String</span></span>|<span data-ttu-id="74f2e-134">Android ストアアカウントのエンタープライズ設定識別子</span><span class="sxs-lookup"><span data-stu-id="74f2e-134">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="74f2e-135">bindStatus</span><span class="sxs-lookup"><span data-stu-id="74f2e-135">bindStatus</span></span>|[<span data-ttu-id="74f2e-136">androidmanagedstoreaccountbindstatus</span><span class="sxs-lookup"><span data-stu-id="74f2e-136">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="74f2e-137">Google EMM API を使用して、テナントの状態をバインドします。</span><span class="sxs-lookup"><span data-stu-id="74f2e-137">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="74f2e-138">使用可能な値は、`notBound`、`bound`、`boundAndValidated`、`unbinding` です。</span><span class="sxs-lookup"><span data-stu-id="74f2e-138">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="74f2e-139">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="74f2e-139">lastAppSyncDateTime</span></span>|<span data-ttu-id="74f2e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74f2e-140">DateTimeOffset</span></span>|<span data-ttu-id="74f2e-141">アプリ同期の最終完了時刻</span><span class="sxs-lookup"><span data-stu-id="74f2e-141">Last completion time for app sync</span></span>|
|<span data-ttu-id="74f2e-142">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="74f2e-142">lastAppSyncStatus</span></span>|[<span data-ttu-id="74f2e-143">androidmanagedstoreaccountappsyncstatus</span><span class="sxs-lookup"><span data-stu-id="74f2e-143">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="74f2e-144">最後のアプリケーションの同期結果。</span><span class="sxs-lookup"><span data-stu-id="74f2e-144">Last application sync result.</span></span> <span data-ttu-id="74f2e-145">使用可能な値: `success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="74f2e-145">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="74f2e-146">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74f2e-146">ownerUserPrincipalName</span></span>|<span data-ttu-id="74f2e-147">String</span><span class="sxs-lookup"><span data-stu-id="74f2e-147">String</span></span>|<span data-ttu-id="74f2e-148">エンタープライズを作成した所有者 UPN</span><span class="sxs-lookup"><span data-stu-id="74f2e-148">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="74f2e-149">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="74f2e-149">ownerOrganizationName</span></span>|<span data-ttu-id="74f2e-150">String</span><span class="sxs-lookup"><span data-stu-id="74f2e-150">String</span></span>|<span data-ttu-id="74f2e-151">Android Enterprise のオンボード時に使用される組織名</span><span class="sxs-lookup"><span data-stu-id="74f2e-151">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="74f2e-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74f2e-152">lastModifiedDateTime</span></span>|<span data-ttu-id="74f2e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74f2e-153">DateTimeOffset</span></span>|<span data-ttu-id="74f2e-154">Android エンタープライズ設定の最終変更時刻</span><span class="sxs-lookup"><span data-stu-id="74f2e-154">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="74f2e-155">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="74f2e-155">enrollmentTarget</span></span>|[<span data-ttu-id="74f2e-156">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="74f2e-156">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="74f2e-157">Android エンタープライズデバイス管理にデバイスを登録できるユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="74f2e-157">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="74f2e-158">使用可能な値は、`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="74f2e-158">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="74f2e-159">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="74f2e-159">targetGroupIds</span></span>|<span data-ttu-id="74f2e-160">String コレクション</span><span class="sxs-lookup"><span data-stu-id="74f2e-160">String collection</span></span>|<span data-ttu-id="74f2e-161">enrollmentTarget が 'Targeted' に設定されている場合、どの AAD グループが Android for Work デバイス管理にデバイスを登録できるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="74f2e-161">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="74f2e-162">deviceownermanagementenabled</span><span class="sxs-lookup"><span data-stu-id="74f2e-162">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="74f2e-163">ブール値</span><span class="sxs-lookup"><span data-stu-id="74f2e-163">Boolean</span></span>|<span data-ttu-id="74f2e-164">CloudDPC を使用した Android デバイス所有者の管理に、このアカウントが flighting になるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74f2e-164">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|
|<span data-ttu-id="74f2e-165">会社コード</span><span class="sxs-lookup"><span data-stu-id="74f2e-165">companyCodes</span></span>|<span data-ttu-id="74f2e-166">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="74f2e-166">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) collection</span></span>|<span data-ttu-id="74f2e-167">androidmanagedstoreaccountenterprisesettings の会社コード</span><span class="sxs-lookup"><span data-stu-id="74f2e-167">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|
|<span data-ttu-id="74f2e-168">androidDeviceOwnerFullyManagedEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="74f2e-168">androidDeviceOwnerFullyManagedEnrollmentEnabled</span></span>|<span data-ttu-id="74f2e-169">ブール値</span><span class="sxs-lookup"><span data-stu-id="74f2e-169">Boolean</span></span>|<span data-ttu-id="74f2e-170">androidmanagedstoreaccountenterprisesettings の会社コード</span><span class="sxs-lookup"><span data-stu-id="74f2e-170">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|



## <a name="response"></a><span data-ttu-id="74f2e-171">応答</span><span class="sxs-lookup"><span data-stu-id="74f2e-171">Response</span></span>
<span data-ttu-id="74f2e-172">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="74f2e-172">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74f2e-173">例</span><span class="sxs-lookup"><span data-stu-id="74f2e-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="74f2e-174">要求</span><span class="sxs-lookup"><span data-stu-id="74f2e-174">Request</span></span>
<span data-ttu-id="74f2e-175">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="74f2e-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="74f2e-176">応答</span><span class="sxs-lookup"><span data-stu-id="74f2e-176">Response</span></span>
<span data-ttu-id="74f2e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="74f2e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




