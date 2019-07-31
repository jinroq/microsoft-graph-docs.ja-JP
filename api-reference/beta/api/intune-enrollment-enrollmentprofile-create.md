---
title: しましたを作成する
description: 新しいしましたオブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f2dac33a8ef52837a148552663049d5953ec61f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985169"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="27c1b-103">しましたを作成する</span><span class="sxs-lookup"><span data-stu-id="27c1b-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="27c1b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27c1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27c1b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="27c1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27c1b-106">新しい[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="27c1b-106">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27c1b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="27c1b-107">Prerequisites</span></span>
<span data-ttu-id="27c1b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27c1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27c1b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27c1b-110">Permission type</span></span>|<span data-ttu-id="27c1b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="27c1b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27c1b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="27c1b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27c1b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27c1b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="27c1b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27c1b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27c1b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27c1b-115">Not supported.</span></span>|
|<span data-ttu-id="27c1b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27c1b-116">Application</span></span>|<span data-ttu-id="27c1b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27c1b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27c1b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27c1b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="27c1b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27c1b-119">Request headers</span></span>
|<span data-ttu-id="27c1b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27c1b-120">Header</span></span>|<span data-ttu-id="27c1b-121">値</span><span class="sxs-lookup"><span data-stu-id="27c1b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27c1b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="27c1b-122">Authorization</span></span>|<span data-ttu-id="27c1b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="27c1b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27c1b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="27c1b-124">Accept</span></span>|<span data-ttu-id="27c1b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27c1b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27c1b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="27c1b-126">Request body</span></span>
<span data-ttu-id="27c1b-127">要求本文で、しましたオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="27c1b-127">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="27c1b-128">次の表に、しましたの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="27c1b-128">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="27c1b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27c1b-129">Property</span></span>|<span data-ttu-id="27c1b-130">型</span><span class="sxs-lookup"><span data-stu-id="27c1b-130">Type</span></span>|<span data-ttu-id="27c1b-131">説明</span><span class="sxs-lookup"><span data-stu-id="27c1b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27c1b-132">id</span><span class="sxs-lookup"><span data-stu-id="27c1b-132">id</span></span>|<span data-ttu-id="27c1b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="27c1b-133">String</span></span>|<span data-ttu-id="27c1b-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="27c1b-134">The GUID for the object</span></span>|
|<span data-ttu-id="27c1b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="27c1b-135">displayName</span></span>|<span data-ttu-id="27c1b-136">String</span><span class="sxs-lookup"><span data-stu-id="27c1b-136">String</span></span>|<span data-ttu-id="27c1b-137">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="27c1b-137">Name of the profile</span></span>|
|<span data-ttu-id="27c1b-138">description</span><span class="sxs-lookup"><span data-stu-id="27c1b-138">description</span></span>|<span data-ttu-id="27c1b-139">String</span><span class="sxs-lookup"><span data-stu-id="27c1b-139">String</span></span>|<span data-ttu-id="27c1b-140">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="27c1b-140">Description of the profile</span></span>|
|<span data-ttu-id="27c1b-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="27c1b-141">requiresUserAuthentication</span></span>|<span data-ttu-id="27c1b-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="27c1b-142">Boolean</span></span>|<span data-ttu-id="27c1b-143">プロファイルにユーザー認証が必要かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="27c1b-143">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="27c1b-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="27c1b-144">configurationEndpointUrl</span></span>|<span data-ttu-id="27c1b-145">String</span><span class="sxs-lookup"><span data-stu-id="27c1b-145">String</span></span>|<span data-ttu-id="27c1b-146">登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="27c1b-146">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="27c1b-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="27c1b-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="27c1b-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="27c1b-148">Boolean</span></span>|<span data-ttu-id="27c1b-149">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="27c1b-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="27c1b-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="27c1b-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="27c1b-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="27c1b-151">Boolean</span></span>|<span data-ttu-id="27c1b-152">セットアップアシスタントの登録済みデバイスで会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="27c1b-152">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="27c1b-153">応答</span><span class="sxs-lookup"><span data-stu-id="27c1b-153">Response</span></span>
<span data-ttu-id="27c1b-154">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="27c1b-154">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27c1b-155">例</span><span class="sxs-lookup"><span data-stu-id="27c1b-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="27c1b-156">要求</span><span class="sxs-lookup"><span data-stu-id="27c1b-156">Request</span></span>
<span data-ttu-id="27c1b-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="27c1b-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 370

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```

### <a name="response"></a><span data-ttu-id="27c1b-158">応答</span><span class="sxs-lookup"><span data-stu-id="27c1b-158">Response</span></span>
<span data-ttu-id="27c1b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="27c1b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 419

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```





