---
title: EnrollmentProfile を更新します。
description: EnrollmentProfile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 85cceaaaaa66822340539c38f6ab8ecde88eae1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400740"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="0da95-103">EnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="0da95-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="0da95-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0da95-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0da95-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0da95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0da95-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0da95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0da95-107">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0da95-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0da95-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0da95-108">Prerequisites</span></span>
<span data-ttu-id="0da95-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0da95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0da95-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0da95-111">Permission type</span></span>|<span data-ttu-id="0da95-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0da95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0da95-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0da95-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0da95-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0da95-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0da95-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0da95-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0da95-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0da95-116">Not supported.</span></span>|
|<span data-ttu-id="0da95-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0da95-117">Application</span></span>|<span data-ttu-id="0da95-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0da95-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0da95-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0da95-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="0da95-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0da95-120">Request headers</span></span>
|<span data-ttu-id="0da95-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0da95-121">Header</span></span>|<span data-ttu-id="0da95-122">値</span><span class="sxs-lookup"><span data-stu-id="0da95-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0da95-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0da95-123">Authorization</span></span>|<span data-ttu-id="0da95-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0da95-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0da95-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0da95-125">Accept</span></span>|<span data-ttu-id="0da95-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0da95-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0da95-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0da95-127">Request body</span></span>
<span data-ttu-id="0da95-128">要求の本文に[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="0da95-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="0da95-129">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="0da95-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="0da95-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0da95-130">Property</span></span>|<span data-ttu-id="0da95-131">型</span><span class="sxs-lookup"><span data-stu-id="0da95-131">Type</span></span>|<span data-ttu-id="0da95-132">説明</span><span class="sxs-lookup"><span data-stu-id="0da95-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0da95-133">id</span><span class="sxs-lookup"><span data-stu-id="0da95-133">id</span></span>|<span data-ttu-id="0da95-134">String</span><span class="sxs-lookup"><span data-stu-id="0da95-134">String</span></span>|<span data-ttu-id="0da95-135">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="0da95-135">The GUID for the object</span></span>|
|<span data-ttu-id="0da95-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0da95-136">displayName</span></span>|<span data-ttu-id="0da95-137">String</span><span class="sxs-lookup"><span data-stu-id="0da95-137">String</span></span>|<span data-ttu-id="0da95-138">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="0da95-138">Name of the profile</span></span>|
|<span data-ttu-id="0da95-139">説明</span><span class="sxs-lookup"><span data-stu-id="0da95-139">description</span></span>|<span data-ttu-id="0da95-140">String</span><span class="sxs-lookup"><span data-stu-id="0da95-140">String</span></span>|<span data-ttu-id="0da95-141">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="0da95-141">Description of the profile</span></span>|
|<span data-ttu-id="0da95-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="0da95-142">requiresUserAuthentication</span></span>|<span data-ttu-id="0da95-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="0da95-143">Boolean</span></span>|<span data-ttu-id="0da95-144">プロファイルにユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="0da95-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="0da95-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="0da95-145">configurationEndpointUrl</span></span>|<span data-ttu-id="0da95-146">String</span><span class="sxs-lookup"><span data-stu-id="0da95-146">String</span></span>|<span data-ttu-id="0da95-147">登録に使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="0da95-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="0da95-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="0da95-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="0da95-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="0da95-149">Boolean</span></span>|<span data-ttu-id="0da95-150">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="0da95-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="0da95-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="0da95-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="0da95-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="0da95-152">Boolean</span></span>|<span data-ttu-id="0da95-153">セットアップ アシスタントが登録されているデバイス上の会社のポータルが必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="0da95-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="0da95-154">応答</span><span class="sxs-lookup"><span data-stu-id="0da95-154">Response</span></span>
<span data-ttu-id="0da95-155">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0da95-155">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0da95-156">例</span><span class="sxs-lookup"><span data-stu-id="0da95-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="0da95-157">要求</span><span class="sxs-lookup"><span data-stu-id="0da95-157">Request</span></span>
<span data-ttu-id="0da95-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0da95-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0da95-159">応答</span><span class="sxs-lookup"><span data-stu-id="0da95-159">Response</span></span>
<span data-ttu-id="0da95-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0da95-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




