---
title: EnrollmentProfile を作成します。
description: 新しい enrollmentProfile オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2a7bb3fb49b57f38ad938f7d43f28f4ece3fda92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414768"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="cc7e3-103">EnrollmentProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="cc7e3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cc7e3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc7e3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc7e3-107">新しい[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-107">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc7e3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="cc7e3-108">Prerequisites</span></span>
<span data-ttu-id="cc7e3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cc7e3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc7e3-111">Permission type</span></span>|<span data-ttu-id="cc7e3-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc7e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc7e3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc7e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc7e3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc7e3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cc7e3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc7e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc7e3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-116">Not supported.</span></span>|
|<span data-ttu-id="cc7e3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc7e3-117">Application</span></span>|<span data-ttu-id="cc7e3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc7e3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc7e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="cc7e3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc7e3-120">Request headers</span></span>
|<span data-ttu-id="cc7e3-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc7e3-121">Header</span></span>|<span data-ttu-id="cc7e3-122">値</span><span class="sxs-lookup"><span data-stu-id="cc7e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc7e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc7e3-123">Authorization</span></span>|<span data-ttu-id="cc7e3-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc7e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cc7e3-125">Accept</span></span>|<span data-ttu-id="cc7e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc7e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc7e3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc7e3-127">Request body</span></span>
<span data-ttu-id="cc7e3-128">要求の本文に enrollmentProfile オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-128">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="cc7e3-129">次の表は、enrollmentProfile を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-129">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="cc7e3-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc7e3-130">Property</span></span>|<span data-ttu-id="cc7e3-131">型</span><span class="sxs-lookup"><span data-stu-id="cc7e3-131">Type</span></span>|<span data-ttu-id="cc7e3-132">説明</span><span class="sxs-lookup"><span data-stu-id="cc7e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc7e3-133">id</span><span class="sxs-lookup"><span data-stu-id="cc7e3-133">id</span></span>|<span data-ttu-id="cc7e3-134">String</span><span class="sxs-lookup"><span data-stu-id="cc7e3-134">String</span></span>|<span data-ttu-id="cc7e3-135">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="cc7e3-135">The GUID for the object</span></span>|
|<span data-ttu-id="cc7e3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cc7e3-136">displayName</span></span>|<span data-ttu-id="cc7e3-137">String</span><span class="sxs-lookup"><span data-stu-id="cc7e3-137">String</span></span>|<span data-ttu-id="cc7e3-138">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="cc7e3-138">Name of the profile</span></span>|
|<span data-ttu-id="cc7e3-139">説明</span><span class="sxs-lookup"><span data-stu-id="cc7e3-139">description</span></span>|<span data-ttu-id="cc7e3-140">String</span><span class="sxs-lookup"><span data-stu-id="cc7e3-140">String</span></span>|<span data-ttu-id="cc7e3-141">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="cc7e3-141">Description of the profile</span></span>|
|<span data-ttu-id="cc7e3-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="cc7e3-142">requiresUserAuthentication</span></span>|<span data-ttu-id="cc7e3-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc7e3-143">Boolean</span></span>|<span data-ttu-id="cc7e3-144">プロファイルにユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="cc7e3-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="cc7e3-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="cc7e3-145">configurationEndpointUrl</span></span>|<span data-ttu-id="cc7e3-146">String</span><span class="sxs-lookup"><span data-stu-id="cc7e3-146">String</span></span>|<span data-ttu-id="cc7e3-147">登録に使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="cc7e3-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="cc7e3-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="cc7e3-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="cc7e3-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc7e3-149">Boolean</span></span>|<span data-ttu-id="cc7e3-150">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="cc7e3-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="cc7e3-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="cc7e3-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc7e3-152">Boolean</span></span>|<span data-ttu-id="cc7e3-153">セットアップ アシスタントが登録されているデバイス上の会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="cc7e3-154">応答</span><span class="sxs-lookup"><span data-stu-id="cc7e3-154">Response</span></span>
<span data-ttu-id="cc7e3-155">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-155">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc7e3-156">例</span><span class="sxs-lookup"><span data-stu-id="cc7e3-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc7e3-157">要求</span><span class="sxs-lookup"><span data-stu-id="cc7e3-157">Request</span></span>
<span data-ttu-id="cc7e3-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cc7e3-159">応答</span><span class="sxs-lookup"><span data-stu-id="cc7e3-159">Response</span></span>
<span data-ttu-id="cc7e3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cc7e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




