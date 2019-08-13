---
title: しましたを作成する
description: 新しいしましたオブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3f50e715b1901bda703ebb6437c7d9d7f6bea9d7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348180"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="67c28-103">しましたを作成する</span><span class="sxs-lookup"><span data-stu-id="67c28-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="67c28-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67c28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67c28-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="67c28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67c28-106">新しい[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="67c28-106">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67c28-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="67c28-107">Prerequisites</span></span>
<span data-ttu-id="67c28-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67c28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67c28-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67c28-110">Permission type</span></span>|<span data-ttu-id="67c28-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="67c28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67c28-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67c28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67c28-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67c28-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="67c28-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67c28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67c28-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67c28-115">Not supported.</span></span>|
|<span data-ttu-id="67c28-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67c28-116">Application</span></span>|<span data-ttu-id="67c28-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67c28-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67c28-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67c28-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="67c28-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67c28-119">Request headers</span></span>
|<span data-ttu-id="67c28-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67c28-120">Header</span></span>|<span data-ttu-id="67c28-121">値</span><span class="sxs-lookup"><span data-stu-id="67c28-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67c28-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="67c28-122">Authorization</span></span>|<span data-ttu-id="67c28-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="67c28-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67c28-124">承諾</span><span class="sxs-lookup"><span data-stu-id="67c28-124">Accept</span></span>|<span data-ttu-id="67c28-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67c28-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67c28-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="67c28-126">Request body</span></span>
<span data-ttu-id="67c28-127">要求本文で、しましたオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="67c28-127">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="67c28-128">次の表に、しましたの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="67c28-128">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="67c28-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67c28-129">Property</span></span>|<span data-ttu-id="67c28-130">型</span><span class="sxs-lookup"><span data-stu-id="67c28-130">Type</span></span>|<span data-ttu-id="67c28-131">説明</span><span class="sxs-lookup"><span data-stu-id="67c28-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67c28-132">id</span><span class="sxs-lookup"><span data-stu-id="67c28-132">id</span></span>|<span data-ttu-id="67c28-133">文字列</span><span class="sxs-lookup"><span data-stu-id="67c28-133">String</span></span>|<span data-ttu-id="67c28-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="67c28-134">The GUID for the object</span></span>|
|<span data-ttu-id="67c28-135">displayName</span><span class="sxs-lookup"><span data-stu-id="67c28-135">displayName</span></span>|<span data-ttu-id="67c28-136">String</span><span class="sxs-lookup"><span data-stu-id="67c28-136">String</span></span>|<span data-ttu-id="67c28-137">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="67c28-137">Name of the profile</span></span>|
|<span data-ttu-id="67c28-138">description</span><span class="sxs-lookup"><span data-stu-id="67c28-138">description</span></span>|<span data-ttu-id="67c28-139">String</span><span class="sxs-lookup"><span data-stu-id="67c28-139">String</span></span>|<span data-ttu-id="67c28-140">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="67c28-140">Description of the profile</span></span>|
|<span data-ttu-id="67c28-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="67c28-141">requiresUserAuthentication</span></span>|<span data-ttu-id="67c28-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c28-142">Boolean</span></span>|<span data-ttu-id="67c28-143">プロファイルにユーザー認証が必要かどうかを示します</span><span class="sxs-lookup"><span data-stu-id="67c28-143">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="67c28-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="67c28-144">configurationEndpointUrl</span></span>|<span data-ttu-id="67c28-145">String</span><span class="sxs-lookup"><span data-stu-id="67c28-145">String</span></span>|<span data-ttu-id="67c28-146">登録に使用する構成エンドポイント url</span><span class="sxs-lookup"><span data-stu-id="67c28-146">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="67c28-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="67c28-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="67c28-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c28-148">Boolean</span></span>|<span data-ttu-id="67c28-149">会社のポータルではなく、Apple セットアップアシスタントを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="67c28-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="67c28-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="67c28-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="67c28-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c28-151">Boolean</span></span>|<span data-ttu-id="67c28-152">セットアップアシスタントの登録済みデバイスで会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="67c28-152">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="67c28-153">応答</span><span class="sxs-lookup"><span data-stu-id="67c28-153">Response</span></span>
<span data-ttu-id="67c28-154">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[しました](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="67c28-154">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67c28-155">例</span><span class="sxs-lookup"><span data-stu-id="67c28-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="67c28-156">要求</span><span class="sxs-lookup"><span data-stu-id="67c28-156">Request</span></span>
<span data-ttu-id="67c28-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67c28-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67c28-158">応答</span><span class="sxs-lookup"><span data-stu-id="67c28-158">Response</span></span>
<span data-ttu-id="67c28-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67c28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






