---
title: しましたの更新
description: しましたオブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a7a34c7e571eadda316631937a718d5907096dab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985113"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="c3518-103">しましたの更新</span><span class="sxs-lookup"><span data-stu-id="c3518-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="c3518-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3518-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3518-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3518-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3518-106">[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c3518-106">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3518-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c3518-107">Prerequisites</span></span>
<span data-ttu-id="c3518-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3518-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3518-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3518-110">Permission type</span></span>|<span data-ttu-id="c3518-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3518-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3518-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3518-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3518-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3518-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c3518-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3518-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3518-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3518-115">Not supported.</span></span>|
|<span data-ttu-id="c3518-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3518-116">Application</span></span>|<span data-ttu-id="c3518-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3518-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3518-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3518-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="c3518-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3518-119">Request headers</span></span>
|<span data-ttu-id="c3518-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3518-120">Header</span></span>|<span data-ttu-id="c3518-121">値</span><span class="sxs-lookup"><span data-stu-id="c3518-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3518-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3518-122">Authorization</span></span>|<span data-ttu-id="c3518-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3518-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3518-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c3518-124">Accept</span></span>|<span data-ttu-id="c3518-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3518-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3518-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3518-126">Request body</span></span>
<span data-ttu-id="c3518-127">要求本文で、[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3518-127">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="c3518-128">次の表に、[しました](../resources/intune-enrollment-enrollmentprofile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c3518-128">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="c3518-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3518-129">Property</span></span>|<span data-ttu-id="c3518-130">型</span><span class="sxs-lookup"><span data-stu-id="c3518-130">Type</span></span>|<span data-ttu-id="c3518-131">説明</span><span class="sxs-lookup"><span data-stu-id="c3518-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3518-132">id</span><span class="sxs-lookup"><span data-stu-id="c3518-132">id</span></span>|<span data-ttu-id="c3518-133">文字列</span><span class="sxs-lookup"><span data-stu-id="c3518-133">String</span></span>|<span data-ttu-id="c3518-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="c3518-134">The GUID for the object</span></span>|
|<span data-ttu-id="c3518-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c3518-135">displayName</span></span>|<span data-ttu-id="c3518-136">String</span><span class="sxs-lookup"><span data-stu-id="c3518-136">String</span></span>|<span data-ttu-id="c3518-137">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="c3518-137">Name of the profile</span></span>|
|<span data-ttu-id="c3518-138">description</span><span class="sxs-lookup"><span data-stu-id="c3518-138">description</span></span>|<span data-ttu-id="c3518-139">String</span><span class="sxs-lookup"><span data-stu-id="c3518-139">String</span></span>|<span data-ttu-id="c3518-140">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="c3518-140">Description of the profile</span></span>|
|<span data-ttu-id="c3518-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="c3518-141">requiresUserAuthentication</span></span>|<span data-ttu-id="c3518-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3518-142">Boolean</span></span>|<span data-ttu-id="c3518-143">プロファイルにユーザー認証が必要かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="c3518-143">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="c3518-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="c3518-144">configurationEndpointUrl</span></span>|<span data-ttu-id="c3518-145">String</span><span class="sxs-lookup"><span data-stu-id="c3518-145">String</span></span>|<span data-ttu-id="c3518-146">登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="c3518-146">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="c3518-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="c3518-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="c3518-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3518-148">Boolean</span></span>|<span data-ttu-id="c3518-149">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="c3518-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="c3518-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="c3518-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="c3518-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3518-151">Boolean</span></span>|<span data-ttu-id="c3518-152">セットアップアシスタントの登録済みデバイスで会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="c3518-152">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="c3518-153">応答</span><span class="sxs-lookup"><span data-stu-id="c3518-153">Response</span></span>
<span data-ttu-id="c3518-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c3518-154">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3518-155">例</span><span class="sxs-lookup"><span data-stu-id="c3518-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3518-156">要求</span><span class="sxs-lookup"><span data-stu-id="c3518-156">Request</span></span>
<span data-ttu-id="c3518-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3518-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
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

### <a name="response"></a><span data-ttu-id="c3518-158">応答</span><span class="sxs-lookup"><span data-stu-id="c3518-158">Response</span></span>
<span data-ttu-id="c3518-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3518-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





