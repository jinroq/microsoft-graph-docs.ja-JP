---
title: EnrollmentProfile を更新します。
description: EnrollmentProfile オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 1f268d07e3636682d77edb238c59e2acaa7ec7d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308317"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="91939-103">EnrollmentProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="91939-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="91939-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="91939-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91939-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91939-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91939-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="91939-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91939-107">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="91939-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="91939-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="91939-108">Prerequisites</span></span>
<span data-ttu-id="91939-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91939-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91939-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91939-111">Permission type</span></span>|<span data-ttu-id="91939-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="91939-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91939-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91939-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91939-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91939-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="91939-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91939-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91939-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91939-116">Not supported.</span></span>|
|<span data-ttu-id="91939-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91939-117">Application</span></span>|<span data-ttu-id="91939-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91939-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91939-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91939-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="91939-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91939-120">Request headers</span></span>
|<span data-ttu-id="91939-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91939-121">Header</span></span>|<span data-ttu-id="91939-122">値</span><span class="sxs-lookup"><span data-stu-id="91939-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91939-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="91939-123">Authorization</span></span>|<span data-ttu-id="91939-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="91939-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91939-125">Accept</span><span class="sxs-lookup"><span data-stu-id="91939-125">Accept</span></span>|<span data-ttu-id="91939-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91939-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91939-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="91939-127">Request body</span></span>
<span data-ttu-id="91939-128">要求の本文に[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="91939-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="91939-129">[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="91939-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="91939-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91939-130">Property</span></span>|<span data-ttu-id="91939-131">種類</span><span class="sxs-lookup"><span data-stu-id="91939-131">Type</span></span>|<span data-ttu-id="91939-132">説明</span><span class="sxs-lookup"><span data-stu-id="91939-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91939-133">ID</span><span class="sxs-lookup"><span data-stu-id="91939-133">id</span></span>|<span data-ttu-id="91939-134">String</span><span class="sxs-lookup"><span data-stu-id="91939-134">String</span></span>|<span data-ttu-id="91939-135">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="91939-135">The GUID for the object</span></span>|
|<span data-ttu-id="91939-136">displayName</span><span class="sxs-lookup"><span data-stu-id="91939-136">displayName</span></span>|<span data-ttu-id="91939-137">String</span><span class="sxs-lookup"><span data-stu-id="91939-137">String</span></span>|<span data-ttu-id="91939-138">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="91939-138">Name of the profile</span></span>|
|<span data-ttu-id="91939-139">説明</span><span class="sxs-lookup"><span data-stu-id="91939-139">description</span></span>|<span data-ttu-id="91939-140">String</span><span class="sxs-lookup"><span data-stu-id="91939-140">String</span></span>|<span data-ttu-id="91939-141">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="91939-141">Description of the profile</span></span>|
|<span data-ttu-id="91939-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="91939-142">requiresUserAuthentication</span></span>|<span data-ttu-id="91939-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="91939-143">Boolean</span></span>|<span data-ttu-id="91939-144">プロファイルにユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="91939-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="91939-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="91939-145">configurationEndpointUrl</span></span>|<span data-ttu-id="91939-146">String</span><span class="sxs-lookup"><span data-stu-id="91939-146">String</span></span>|<span data-ttu-id="91939-147">登録に使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="91939-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="91939-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="91939-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="91939-149">ブール型</span><span class="sxs-lookup"><span data-stu-id="91939-149">Boolean</span></span>|<span data-ttu-id="91939-150">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="91939-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="91939-151">応答</span><span class="sxs-lookup"><span data-stu-id="91939-151">Response</span></span>
<span data-ttu-id="91939-152">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="91939-152">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91939-153">例</span><span class="sxs-lookup"><span data-stu-id="91939-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="91939-154">要求</span><span class="sxs-lookup"><span data-stu-id="91939-154">Request</span></span>
<span data-ttu-id="91939-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="91939-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 250

{
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```

### <a name="response"></a><span data-ttu-id="91939-156">応答</span><span class="sxs-lookup"><span data-stu-id="91939-156">Response</span></span>
<span data-ttu-id="91939-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="91939-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```





