---
title: Create vppToken
description: 新規にvppTokenオブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 713a6bf583ff9c315ec88a83811312e6a6af5d92
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980475"
---
# <a name="create-vpptoken"></a><span data-ttu-id="2965c-103">Create vppToken</span><span class="sxs-lookup"><span data-stu-id="2965c-103">Create vppToken</span></span>

> <span data-ttu-id="2965c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2965c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2965c-105">新規に[vppToken](../resources/intune-onboarding-vpptoken.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2965c-105">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2965c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="2965c-106">Prerequisites</span></span>
<span data-ttu-id="2965c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2965c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2965c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2965c-109">Permission type</span></span>|<span data-ttu-id="2965c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2965c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2965c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2965c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2965c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2965c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2965c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2965c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2965c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2965c-114">Not supported.</span></span>|
|<span data-ttu-id="2965c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2965c-115">Application</span></span>|<span data-ttu-id="2965c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2965c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2965c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2965c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="2965c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2965c-118">Request headers</span></span>
|<span data-ttu-id="2965c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2965c-119">Header</span></span>|<span data-ttu-id="2965c-120">値</span><span class="sxs-lookup"><span data-stu-id="2965c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2965c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2965c-121">Authorization</span></span>|<span data-ttu-id="2965c-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2965c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2965c-123">承諾</span><span class="sxs-lookup"><span data-stu-id="2965c-123">Accept</span></span>|<span data-ttu-id="2965c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2965c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2965c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2965c-125">Request body</span></span>
<span data-ttu-id="2965c-126">要求本文で、vppToken オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2965c-126">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="2965c-127">次の表に、vppToken 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2965c-127">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="2965c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2965c-128">Property</span></span>|<span data-ttu-id="2965c-129">型</span><span class="sxs-lookup"><span data-stu-id="2965c-129">Type</span></span>|<span data-ttu-id="2965c-130">説明</span><span class="sxs-lookup"><span data-stu-id="2965c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2965c-131">id</span><span class="sxs-lookup"><span data-stu-id="2965c-131">id</span></span>|<span data-ttu-id="2965c-132">String</span><span class="sxs-lookup"><span data-stu-id="2965c-132">String</span></span>|<span data-ttu-id="2965c-133">appleVolumePurchaseProgramToken 作成時に自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="2965c-133">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="2965c-134">エンティティのキーになります。</span><span class="sxs-lookup"><span data-stu-id="2965c-134">It is the Key of the entity.</span></span>|
|<span data-ttu-id="2965c-135">organizationName</span><span class="sxs-lookup"><span data-stu-id="2965c-135">organizationName</span></span>|<span data-ttu-id="2965c-136">String</span><span class="sxs-lookup"><span data-stu-id="2965c-136">String</span></span>|<span data-ttu-id="2965c-137">Apple ボリューム購入プログラムのトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="2965c-137">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="2965c-138">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2965c-138">vppTokenAccountType</span></span>|[<span data-ttu-id="2965c-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2965c-139">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="2965c-140">特定の Apple ボリューム購入プログラムのトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="2965c-140">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="2965c-141">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="2965c-141">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="2965c-142">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="2965c-142">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="2965c-143">appleId</span><span class="sxs-lookup"><span data-stu-id="2965c-143">appleId</span></span>|<span data-ttu-id="2965c-144">String</span><span class="sxs-lookup"><span data-stu-id="2965c-144">String</span></span>|<span data-ttu-id="2965c-145">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="2965c-145">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2965c-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2965c-146">expirationDateTime</span></span>|<span data-ttu-id="2965c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2965c-147">DateTimeOffset</span></span>|<span data-ttu-id="2965c-148">Apple ボリューム購入プログラムのトークンの有効期限。</span><span class="sxs-lookup"><span data-stu-id="2965c-148">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2965c-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2965c-149">lastSyncDateTime</span></span>|<span data-ttu-id="2965c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2965c-150">DateTimeOffset</span></span>|<span data-ttu-id="2965c-151">Apple ボリューム購入プログラムのトークンを使用して、Apple ボリューム購入プログラム サービスと最後にアプリケーションの同期を行った日時。</span><span class="sxs-lookup"><span data-stu-id="2965c-151">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2965c-152">token</span><span class="sxs-lookup"><span data-stu-id="2965c-152">token</span></span>|<span data-ttu-id="2965c-153">String</span><span class="sxs-lookup"><span data-stu-id="2965c-153">String</span></span>|<span data-ttu-id="2965c-154">Apple ボリューム購入プログラムからダウンロードした Apple ボリューム購入プログラムのトークン文字列。</span><span class="sxs-lookup"><span data-stu-id="2965c-154">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="2965c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2965c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="2965c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2965c-156">DateTimeOffset</span></span>|<span data-ttu-id="2965c-157">Apple ボリューム購入プログラムのトークンに関連付けられている最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="2965c-157">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2965c-158">state</span><span class="sxs-lookup"><span data-stu-id="2965c-158">state</span></span>|[<span data-ttu-id="2965c-159">vpptokenstate</span><span class="sxs-lookup"><span data-stu-id="2965c-159">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="2965c-160">Apple ボリューム購入プログラムのトークンの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="2965c-160">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="2965c-161">可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。</span><span class="sxs-lookup"><span data-stu-id="2965c-161">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="2965c-162">可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。</span><span class="sxs-lookup"><span data-stu-id="2965c-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="2965c-163">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="2965c-163">lastSyncStatus</span></span>|[<span data-ttu-id="2965c-164">vpptokensyncstatus</span><span class="sxs-lookup"><span data-stu-id="2965c-164">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="2965c-165">Apple ボリューム購入プログラム トークンを使用して行われた最後のアプリケーションの同期の現在の同期状態。</span><span class="sxs-lookup"><span data-stu-id="2965c-165">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="2965c-166">可能な値は、`none`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="2965c-166">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="2965c-167">可能な値は、`none`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="2965c-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="2965c-168">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="2965c-168">automaticallyUpdateApps</span></span>|<span data-ttu-id="2965c-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="2965c-169">Boolean</span></span>|<span data-ttu-id="2965c-170">VPP トークンのアプリを自動で更新するかどうか。</span><span class="sxs-lookup"><span data-stu-id="2965c-170">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="2965c-171">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="2965c-171">countryOrRegion</span></span>|<span data-ttu-id="2965c-172">文字列</span><span class="sxs-lookup"><span data-stu-id="2965c-172">String</span></span>|<span data-ttu-id="2965c-173">VPP トークンのアプリを自動で更新するかどうか。</span><span class="sxs-lookup"><span data-stu-id="2965c-173">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="2965c-174">応答</span><span class="sxs-lookup"><span data-stu-id="2965c-174">Response</span></span>
<span data-ttu-id="2965c-175">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [vppToken](../resources/intune-onboarding-vpptoken.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2965c-175">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2965c-176">例</span><span class="sxs-lookup"><span data-stu-id="2965c-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="2965c-177">要求</span><span class="sxs-lookup"><span data-stu-id="2965c-177">Request</span></span>
<span data-ttu-id="2965c-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2965c-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 461

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a><span data-ttu-id="2965c-179">応答</span><span class="sxs-lookup"><span data-stu-id="2965c-179">Response</span></span>
<span data-ttu-id="2965c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2965c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

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
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```



