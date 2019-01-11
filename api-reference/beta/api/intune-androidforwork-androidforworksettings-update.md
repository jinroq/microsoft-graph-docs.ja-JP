---
title: Update androidForWorkSettings
description: androidForWorkSettings オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b46daa868d240b7ae50c83d708b8bf744e8079be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849764"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="9fe41-103">Update androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="9fe41-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="9fe41-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9fe41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fe41-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fe41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9fe41-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9fe41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fe41-107">[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9fe41-107">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9fe41-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9fe41-108">Prerequisites</span></span>
<span data-ttu-id="9fe41-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9fe41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fe41-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9fe41-111">Permission type</span></span>|<span data-ttu-id="9fe41-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9fe41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fe41-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9fe41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fe41-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fe41-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9fe41-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9fe41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fe41-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fe41-116">Not supported.</span></span>|
|<span data-ttu-id="9fe41-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9fe41-117">Application</span></span>|<span data-ttu-id="9fe41-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fe41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fe41-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9fe41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="9fe41-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9fe41-120">Request headers</span></span>
|<span data-ttu-id="9fe41-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9fe41-121">Header</span></span>|<span data-ttu-id="9fe41-122">値</span><span class="sxs-lookup"><span data-stu-id="9fe41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fe41-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fe41-123">Authorization</span></span>|<span data-ttu-id="9fe41-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9fe41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fe41-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9fe41-125">Accept</span></span>|<span data-ttu-id="9fe41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fe41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fe41-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9fe41-127">Request body</span></span>
<span data-ttu-id="9fe41-128">要求本文で、[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9fe41-128">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="9fe41-129">次の表に、[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9fe41-129">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="9fe41-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9fe41-130">Property</span></span>|<span data-ttu-id="9fe41-131">種類</span><span class="sxs-lookup"><span data-stu-id="9fe41-131">Type</span></span>|<span data-ttu-id="9fe41-132">説明</span><span class="sxs-lookup"><span data-stu-id="9fe41-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fe41-133">ID</span><span class="sxs-lookup"><span data-stu-id="9fe41-133">id</span></span>|<span data-ttu-id="9fe41-134">String</span><span class="sxs-lookup"><span data-stu-id="9fe41-134">String</span></span>|<span data-ttu-id="9fe41-135">Android for Work 設定の識別子</span><span class="sxs-lookup"><span data-stu-id="9fe41-135">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="9fe41-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="9fe41-136">bindStatus</span></span>|[<span data-ttu-id="9fe41-137">androidForWorkBindStatus</span><span class="sxs-lookup"><span data-stu-id="9fe41-137">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="9fe41-138">Google の EMM の API を使用してテナントの状態をバインドします。</span><span class="sxs-lookup"><span data-stu-id="9fe41-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="9fe41-139">可能な値は、`notBound`、`bound`、`boundAndValidated`、`unbinding` です。</span><span class="sxs-lookup"><span data-stu-id="9fe41-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="9fe41-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9fe41-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="9fe41-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fe41-141">DateTimeOffset</span></span>|<span data-ttu-id="9fe41-142">アプリ同期の最終完了時刻</span><span class="sxs-lookup"><span data-stu-id="9fe41-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="9fe41-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="9fe41-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="9fe41-144">androidForWorkSyncStatus</span><span class="sxs-lookup"><span data-stu-id="9fe41-144">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="9fe41-145">アプリケーション同期の最終結果です。</span><span class="sxs-lookup"><span data-stu-id="9fe41-145">Last application sync result.</span></span> <span data-ttu-id="9fe41-146">使用可能な値: `success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="9fe41-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="9fe41-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9fe41-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="9fe41-148">String</span><span class="sxs-lookup"><span data-stu-id="9fe41-148">String</span></span>|<span data-ttu-id="9fe41-149">エンタープライズを作成した所有者 UPN</span><span class="sxs-lookup"><span data-stu-id="9fe41-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="9fe41-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="9fe41-150">ownerOrganizationName</span></span>|<span data-ttu-id="9fe41-151">String</span><span class="sxs-lookup"><span data-stu-id="9fe41-151">String</span></span>|<span data-ttu-id="9fe41-152">Android for Work の配布準備時に使用される組織名</span><span class="sxs-lookup"><span data-stu-id="9fe41-152">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="9fe41-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fe41-153">lastModifiedDateTime</span></span>|<span data-ttu-id="9fe41-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fe41-154">DateTimeOffset</span></span>|<span data-ttu-id="9fe41-155">Android for Work 設定の最終変更時刻</span><span class="sxs-lookup"><span data-stu-id="9fe41-155">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="9fe41-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="9fe41-156">enrollmentTarget</span></span>|[<span data-ttu-id="9fe41-157">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="9fe41-157">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="9fe41-158">ワーク デバイス管理のアプリでデバイスを登録できるユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="9fe41-158">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="9fe41-159">可能な値は、`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="9fe41-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="9fe41-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="9fe41-160">targetGroupIds</span></span>|<span data-ttu-id="9fe41-161">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9fe41-161">String collection</span></span>|<span data-ttu-id="9fe41-162">enrollmentTarget が 'Targeted' に設定されている場合、どの AAD グループが Android for Work デバイス管理にデバイスを登録できるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9fe41-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="9fe41-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="9fe41-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="9fe41-164">ブール型</span><span class="sxs-lookup"><span data-stu-id="9fe41-164">Boolean</span></span>|<span data-ttu-id="9fe41-165">このアカウントを CloudDPC に Android のデバイスの所有者の管理の flighting かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9fe41-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="9fe41-166">応答</span><span class="sxs-lookup"><span data-stu-id="9fe41-166">Response</span></span>
<span data-ttu-id="9fe41-167">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="9fe41-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fe41-168">例</span><span class="sxs-lookup"><span data-stu-id="9fe41-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="9fe41-169">要求</span><span class="sxs-lookup"><span data-stu-id="9fe41-169">Request</span></span>
<span data-ttu-id="9fe41-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9fe41-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
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

### <a name="response"></a><span data-ttu-id="9fe41-171">応答</span><span class="sxs-lookup"><span data-stu-id="9fe41-171">Response</span></span>
<span data-ttu-id="9fe41-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9fe41-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





