---
title: AndroidManagedStoreAccountEnterpriseSettings を更新します。
description: AndroidManagedStoreAccountEnterpriseSettings オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e57b7965e5393faf9bdb953dc915652772deb14c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398486"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="818c2-103">AndroidManagedStoreAccountEnterpriseSettings を更新します。</span><span class="sxs-lookup"><span data-stu-id="818c2-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="818c2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="818c2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="818c2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="818c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="818c2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="818c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="818c2-107">[AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="818c2-107">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="818c2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="818c2-108">Prerequisites</span></span>
<span data-ttu-id="818c2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="818c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="818c2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="818c2-111">Permission type</span></span>|<span data-ttu-id="818c2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="818c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="818c2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="818c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="818c2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="818c2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="818c2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="818c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="818c2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="818c2-116">Not supported.</span></span>|
|<span data-ttu-id="818c2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="818c2-117">Application</span></span>|<span data-ttu-id="818c2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="818c2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="818c2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="818c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="818c2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="818c2-120">Request headers</span></span>
|<span data-ttu-id="818c2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="818c2-121">Header</span></span>|<span data-ttu-id="818c2-122">値</span><span class="sxs-lookup"><span data-stu-id="818c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="818c2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="818c2-123">Authorization</span></span>|<span data-ttu-id="818c2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="818c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="818c2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="818c2-125">Accept</span></span>|<span data-ttu-id="818c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="818c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="818c2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="818c2-127">Request body</span></span>
<span data-ttu-id="818c2-128">要求の本文に[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="818c2-128">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="818c2-129">[AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="818c2-129">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="818c2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="818c2-130">Property</span></span>|<span data-ttu-id="818c2-131">型</span><span class="sxs-lookup"><span data-stu-id="818c2-131">Type</span></span>|<span data-ttu-id="818c2-132">説明</span><span class="sxs-lookup"><span data-stu-id="818c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="818c2-133">id</span><span class="sxs-lookup"><span data-stu-id="818c2-133">id</span></span>|<span data-ttu-id="818c2-134">String</span><span class="sxs-lookup"><span data-stu-id="818c2-134">String</span></span>|<span data-ttu-id="818c2-135">アカウントのエンタープライズ設定の識別子を格納する、アプリ</span><span class="sxs-lookup"><span data-stu-id="818c2-135">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="818c2-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="818c2-136">bindStatus</span></span>|[<span data-ttu-id="818c2-137">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="818c2-137">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="818c2-138">Google の EMM の API を使用してテナントの状態をバインドします。</span><span class="sxs-lookup"><span data-stu-id="818c2-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="818c2-139">可能な値は、`notBound`、`bound`、`boundAndValidated`、`unbinding` です。</span><span class="sxs-lookup"><span data-stu-id="818c2-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="818c2-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="818c2-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="818c2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="818c2-141">DateTimeOffset</span></span>|<span data-ttu-id="818c2-142">アプリ同期の最終完了時刻</span><span class="sxs-lookup"><span data-stu-id="818c2-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="818c2-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="818c2-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="818c2-144">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="818c2-144">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="818c2-145">アプリケーション同期の最終結果です。</span><span class="sxs-lookup"><span data-stu-id="818c2-145">Last application sync result.</span></span> <span data-ttu-id="818c2-146">使用可能な値: `success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="818c2-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="818c2-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="818c2-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="818c2-148">String</span><span class="sxs-lookup"><span data-stu-id="818c2-148">String</span></span>|<span data-ttu-id="818c2-149">エンタープライズを作成した所有者 UPN</span><span class="sxs-lookup"><span data-stu-id="818c2-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="818c2-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="818c2-150">ownerOrganizationName</span></span>|<span data-ttu-id="818c2-151">String</span><span class="sxs-lookup"><span data-stu-id="818c2-151">String</span></span>|<span data-ttu-id="818c2-152">組織名を使用する場合 Android のエンタープライズ契約時</span><span class="sxs-lookup"><span data-stu-id="818c2-152">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="818c2-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="818c2-153">lastModifiedDateTime</span></span>|<span data-ttu-id="818c2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="818c2-154">DateTimeOffset</span></span>|<span data-ttu-id="818c2-155">Android エンタープライズ設定の最終変更時刻</span><span class="sxs-lookup"><span data-stu-id="818c2-155">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="818c2-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="818c2-156">enrollmentTarget</span></span>|[<span data-ttu-id="818c2-157">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="818c2-157">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="818c2-158">Android エンタープライズ デバイスの管理デバイスを登録できるユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="818c2-158">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="818c2-159">可能な値は、`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="818c2-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="818c2-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="818c2-160">targetGroupIds</span></span>|<span data-ttu-id="818c2-161">String コレクション</span><span class="sxs-lookup"><span data-stu-id="818c2-161">String collection</span></span>|<span data-ttu-id="818c2-162">enrollmentTarget が 'Targeted' に設定されている場合、どの AAD グループが Android for Work デバイス管理にデバイスを登録できるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="818c2-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="818c2-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="818c2-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="818c2-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="818c2-164">Boolean</span></span>|<span data-ttu-id="818c2-165">このアカウントを CloudDPC に Android のデバイスの所有者の管理の flighting かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="818c2-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|
|<span data-ttu-id="818c2-166">companyCodes</span><span class="sxs-lookup"><span data-stu-id="818c2-166">companyCodes</span></span>|<span data-ttu-id="818c2-167">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="818c2-167">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) collection</span></span>|<span data-ttu-id="818c2-168">AndroidManagedStoreAccountEnterpriseSettings の会社コード</span><span class="sxs-lookup"><span data-stu-id="818c2-168">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|
|<span data-ttu-id="818c2-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="818c2-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span></span>|<span data-ttu-id="818c2-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="818c2-170">Boolean</span></span>|<span data-ttu-id="818c2-171">AndroidManagedStoreAccountEnterpriseSettings の会社コード</span><span class="sxs-lookup"><span data-stu-id="818c2-171">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|



## <a name="response"></a><span data-ttu-id="818c2-172">応答</span><span class="sxs-lookup"><span data-stu-id="818c2-172">Response</span></span>
<span data-ttu-id="818c2-173">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="818c2-173">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="818c2-174">例</span><span class="sxs-lookup"><span data-stu-id="818c2-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="818c2-175">要求</span><span class="sxs-lookup"><span data-stu-id="818c2-175">Request</span></span>
<span data-ttu-id="818c2-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="818c2-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="818c2-177">応答</span><span class="sxs-lookup"><span data-stu-id="818c2-177">Response</span></span>
<span data-ttu-id="818c2-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="818c2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




