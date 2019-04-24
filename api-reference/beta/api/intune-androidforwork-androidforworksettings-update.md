---
title: Update androidForWorkSettings
description: androidForWorkSettings オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f71d9087b457189d3796306e0585981c0e58855
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32498215"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="f3593-103">Update androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="f3593-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="f3593-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3593-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3593-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3593-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3593-106">[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f3593-106">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3593-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f3593-107">Prerequisites</span></span>
<span data-ttu-id="f3593-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3593-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3593-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3593-110">Permission type</span></span>|<span data-ttu-id="f3593-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3593-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3593-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3593-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3593-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3593-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3593-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3593-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3593-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3593-115">Not supported.</span></span>|
|<span data-ttu-id="f3593-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3593-116">Application</span></span>|<span data-ttu-id="f3593-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3593-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3593-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3593-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="f3593-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3593-119">Request headers</span></span>
|<span data-ttu-id="f3593-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3593-120">Header</span></span>|<span data-ttu-id="f3593-121">値</span><span class="sxs-lookup"><span data-stu-id="f3593-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3593-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3593-122">Authorization</span></span>|<span data-ttu-id="f3593-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3593-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3593-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f3593-124">Accept</span></span>|<span data-ttu-id="f3593-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3593-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3593-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3593-126">Request body</span></span>
<span data-ttu-id="f3593-127">要求本文で、[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3593-127">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="f3593-128">次の表に、[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f3593-128">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="f3593-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3593-129">Property</span></span>|<span data-ttu-id="f3593-130">型</span><span class="sxs-lookup"><span data-stu-id="f3593-130">Type</span></span>|<span data-ttu-id="f3593-131">説明</span><span class="sxs-lookup"><span data-stu-id="f3593-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3593-132">id</span><span class="sxs-lookup"><span data-stu-id="f3593-132">id</span></span>|<span data-ttu-id="f3593-133">String</span><span class="sxs-lookup"><span data-stu-id="f3593-133">String</span></span>|<span data-ttu-id="f3593-134">Android for Work の設定の識別子</span><span class="sxs-lookup"><span data-stu-id="f3593-134">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="f3593-135">bindStatus</span><span class="sxs-lookup"><span data-stu-id="f3593-135">bindStatus</span></span>|[<span data-ttu-id="f3593-136">androidforwork bindstatus</span><span class="sxs-lookup"><span data-stu-id="f3593-136">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="f3593-137">Google EMM API を使用して、テナントの状態をバインドします。</span><span class="sxs-lookup"><span data-stu-id="f3593-137">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="f3593-138">可能な値は、`notBound`、`bound`、`boundAndValidated`、`unbinding` です。</span><span class="sxs-lookup"><span data-stu-id="f3593-138">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="f3593-139">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f3593-139">lastAppSyncDateTime</span></span>|<span data-ttu-id="f3593-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3593-140">DateTimeOffset</span></span>|<span data-ttu-id="f3593-141">アプリ同期の最終完了時刻</span><span class="sxs-lookup"><span data-stu-id="f3593-141">Last completion time for app sync</span></span>|
|<span data-ttu-id="f3593-142">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="f3593-142">lastAppSyncStatus</span></span>|[<span data-ttu-id="f3593-143">androidforwork syncstatus</span><span class="sxs-lookup"><span data-stu-id="f3593-143">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="f3593-144">最後のアプリケーションの同期結果。</span><span class="sxs-lookup"><span data-stu-id="f3593-144">Last application sync result.</span></span> <span data-ttu-id="f3593-145">可能な値は `success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="f3593-145">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="f3593-146">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f3593-146">ownerUserPrincipalName</span></span>|<span data-ttu-id="f3593-147">String</span><span class="sxs-lookup"><span data-stu-id="f3593-147">String</span></span>|<span data-ttu-id="f3593-148">エンタープライズを作成した所有者の UPN</span><span class="sxs-lookup"><span data-stu-id="f3593-148">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="f3593-149">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="f3593-149">ownerOrganizationName</span></span>|<span data-ttu-id="f3593-150">String</span><span class="sxs-lookup"><span data-stu-id="f3593-150">String</span></span>|<span data-ttu-id="f3593-151">Android for Work のオンボーディング時に使用される組織名</span><span class="sxs-lookup"><span data-stu-id="f3593-151">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="f3593-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3593-152">lastModifiedDateTime</span></span>|<span data-ttu-id="f3593-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3593-153">DateTimeOffset</span></span>|<span data-ttu-id="f3593-154">Android for Work の設定の最終変更時刻</span><span class="sxs-lookup"><span data-stu-id="f3593-154">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="f3593-155">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="f3593-155">enrollmentTarget</span></span>|[<span data-ttu-id="f3593-156">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="f3593-156">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="f3593-157">Android for Work デバイス管理にデバイスを登録できるユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="f3593-157">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="f3593-158">可能な値は、`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="f3593-158">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="f3593-159">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="f3593-159">targetGroupIds</span></span>|<span data-ttu-id="f3593-160">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f3593-160">String collection</span></span>|<span data-ttu-id="f3593-161">enrollmentTarget が「Targeted」に設定されている場合、どの AAD グループが Android for Work デバイス管理にデバイスを登録できるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f3593-161">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="f3593-162">deviceownermanagementenabled</span><span class="sxs-lookup"><span data-stu-id="f3593-162">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="f3593-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3593-163">Boolean</span></span>|<span data-ttu-id="f3593-164">CloudDPC を使用した Android デバイス所有者の管理に、このアカウントが flighting になるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f3593-164">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="f3593-165">応答</span><span class="sxs-lookup"><span data-stu-id="f3593-165">Response</span></span>
<span data-ttu-id="f3593-166">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidforwork settings](../resources/intune-androidforwork-androidforworksettings.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3593-166">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3593-167">例</span><span class="sxs-lookup"><span data-stu-id="f3593-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3593-168">要求</span><span class="sxs-lookup"><span data-stu-id="f3593-168">Request</span></span>
<span data-ttu-id="f3593-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3593-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="f3593-170">応答</span><span class="sxs-lookup"><span data-stu-id="f3593-170">Response</span></span>
<span data-ttu-id="f3593-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3593-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 568

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
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





