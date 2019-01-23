---
title: Update androidForWorkSettings
description: androidForWorkSettings オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7332cc22e32abd3722bb2331c721ef730f0b59b8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401741"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="307a7-103">Update androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="307a7-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="307a7-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="307a7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="307a7-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="307a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="307a7-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="307a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="307a7-107">[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="307a7-107">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="307a7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="307a7-108">Prerequisites</span></span>
<span data-ttu-id="307a7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="307a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="307a7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="307a7-111">Permission type</span></span>|<span data-ttu-id="307a7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="307a7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="307a7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="307a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="307a7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="307a7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="307a7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="307a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="307a7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="307a7-116">Not supported.</span></span>|
|<span data-ttu-id="307a7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="307a7-117">Application</span></span>|<span data-ttu-id="307a7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="307a7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="307a7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="307a7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="307a7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="307a7-120">Request headers</span></span>
|<span data-ttu-id="307a7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="307a7-121">Header</span></span>|<span data-ttu-id="307a7-122">値</span><span class="sxs-lookup"><span data-stu-id="307a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="307a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="307a7-123">Authorization</span></span>|<span data-ttu-id="307a7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="307a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="307a7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="307a7-125">Accept</span></span>|<span data-ttu-id="307a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="307a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="307a7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="307a7-127">Request body</span></span>
<span data-ttu-id="307a7-128">要求本文で、[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="307a7-128">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="307a7-129">次の表に、[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="307a7-129">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="307a7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="307a7-130">Property</span></span>|<span data-ttu-id="307a7-131">型</span><span class="sxs-lookup"><span data-stu-id="307a7-131">Type</span></span>|<span data-ttu-id="307a7-132">説明</span><span class="sxs-lookup"><span data-stu-id="307a7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="307a7-133">id</span><span class="sxs-lookup"><span data-stu-id="307a7-133">id</span></span>|<span data-ttu-id="307a7-134">String</span><span class="sxs-lookup"><span data-stu-id="307a7-134">String</span></span>|<span data-ttu-id="307a7-135">Android for Work 設定の識別子</span><span class="sxs-lookup"><span data-stu-id="307a7-135">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="307a7-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="307a7-136">bindStatus</span></span>|[<span data-ttu-id="307a7-137">androidForWorkBindStatus</span><span class="sxs-lookup"><span data-stu-id="307a7-137">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="307a7-138">Google の EMM の API を使用してテナントの状態をバインドします。</span><span class="sxs-lookup"><span data-stu-id="307a7-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="307a7-139">可能な値は、`notBound`、`bound`、`boundAndValidated`、`unbinding` です。</span><span class="sxs-lookup"><span data-stu-id="307a7-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="307a7-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="307a7-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="307a7-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="307a7-141">DateTimeOffset</span></span>|<span data-ttu-id="307a7-142">アプリ同期の最終完了時刻</span><span class="sxs-lookup"><span data-stu-id="307a7-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="307a7-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="307a7-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="307a7-144">androidForWorkSyncStatus</span><span class="sxs-lookup"><span data-stu-id="307a7-144">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="307a7-145">アプリケーション同期の最終結果です。</span><span class="sxs-lookup"><span data-stu-id="307a7-145">Last application sync result.</span></span> <span data-ttu-id="307a7-146">使用可能な値: `success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="307a7-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="307a7-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="307a7-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="307a7-148">String</span><span class="sxs-lookup"><span data-stu-id="307a7-148">String</span></span>|<span data-ttu-id="307a7-149">エンタープライズを作成した所有者 UPN</span><span class="sxs-lookup"><span data-stu-id="307a7-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="307a7-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="307a7-150">ownerOrganizationName</span></span>|<span data-ttu-id="307a7-151">String</span><span class="sxs-lookup"><span data-stu-id="307a7-151">String</span></span>|<span data-ttu-id="307a7-152">Android for Work の配布準備時に使用される組織名</span><span class="sxs-lookup"><span data-stu-id="307a7-152">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="307a7-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="307a7-153">lastModifiedDateTime</span></span>|<span data-ttu-id="307a7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="307a7-154">DateTimeOffset</span></span>|<span data-ttu-id="307a7-155">Android for Work 設定の最終変更時刻</span><span class="sxs-lookup"><span data-stu-id="307a7-155">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="307a7-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="307a7-156">enrollmentTarget</span></span>|[<span data-ttu-id="307a7-157">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="307a7-157">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="307a7-158">ワーク デバイス管理のアプリでデバイスを登録できるユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="307a7-158">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="307a7-159">可能な値は、`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="307a7-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="307a7-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="307a7-160">targetGroupIds</span></span>|<span data-ttu-id="307a7-161">String コレクション</span><span class="sxs-lookup"><span data-stu-id="307a7-161">String collection</span></span>|<span data-ttu-id="307a7-162">enrollmentTarget が 'Targeted' に設定されている場合、どの AAD グループが Android for Work デバイス管理にデバイスを登録できるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="307a7-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="307a7-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="307a7-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="307a7-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="307a7-164">Boolean</span></span>|<span data-ttu-id="307a7-165">このアカウントを CloudDPC に Android のデバイスの所有者の管理の flighting かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="307a7-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="307a7-166">応答</span><span class="sxs-lookup"><span data-stu-id="307a7-166">Response</span></span>
<span data-ttu-id="307a7-167">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="307a7-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="307a7-168">例</span><span class="sxs-lookup"><span data-stu-id="307a7-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="307a7-169">要求</span><span class="sxs-lookup"><span data-stu-id="307a7-169">Request</span></span>
<span data-ttu-id="307a7-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="307a7-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="307a7-171">応答</span><span class="sxs-lookup"><span data-stu-id="307a7-171">Response</span></span>
<span data-ttu-id="307a7-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="307a7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




