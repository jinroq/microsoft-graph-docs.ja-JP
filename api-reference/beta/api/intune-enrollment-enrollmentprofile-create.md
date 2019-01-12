---
title: EnrollmentProfile を作成します。
description: 新しい enrollmentProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bf4133e636cd9eedf7737e2003d1ba733a6e08ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934143"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="3daa0-103">EnrollmentProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="3daa0-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="3daa0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3daa0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3daa0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3daa0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3daa0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3daa0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3daa0-107">新しい[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3daa0-107">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3daa0-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3daa0-108">Prerequisites</span></span>
<span data-ttu-id="3daa0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3daa0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3daa0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3daa0-111">Permission type</span></span>|<span data-ttu-id="3daa0-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3daa0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3daa0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3daa0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3daa0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3daa0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3daa0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3daa0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3daa0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3daa0-116">Not supported.</span></span>|
|<span data-ttu-id="3daa0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3daa0-117">Application</span></span>|<span data-ttu-id="3daa0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3daa0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3daa0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3daa0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="3daa0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3daa0-120">Request headers</span></span>
|<span data-ttu-id="3daa0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3daa0-121">Header</span></span>|<span data-ttu-id="3daa0-122">値</span><span class="sxs-lookup"><span data-stu-id="3daa0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3daa0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3daa0-123">Authorization</span></span>|<span data-ttu-id="3daa0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3daa0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3daa0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3daa0-125">Accept</span></span>|<span data-ttu-id="3daa0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3daa0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3daa0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3daa0-127">Request body</span></span>
<span data-ttu-id="3daa0-128">要求の本文に enrollmentProfile オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="3daa0-128">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="3daa0-129">次の表は、enrollmentProfile を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3daa0-129">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="3daa0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3daa0-130">Property</span></span>|<span data-ttu-id="3daa0-131">型</span><span class="sxs-lookup"><span data-stu-id="3daa0-131">Type</span></span>|<span data-ttu-id="3daa0-132">説明</span><span class="sxs-lookup"><span data-stu-id="3daa0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3daa0-133">ID</span><span class="sxs-lookup"><span data-stu-id="3daa0-133">id</span></span>|<span data-ttu-id="3daa0-134">String</span><span class="sxs-lookup"><span data-stu-id="3daa0-134">String</span></span>|<span data-ttu-id="3daa0-135">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="3daa0-135">The GUID for the object</span></span>|
|<span data-ttu-id="3daa0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3daa0-136">displayName</span></span>|<span data-ttu-id="3daa0-137">String</span><span class="sxs-lookup"><span data-stu-id="3daa0-137">String</span></span>|<span data-ttu-id="3daa0-138">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="3daa0-138">Name of the profile</span></span>|
|<span data-ttu-id="3daa0-139">説明</span><span class="sxs-lookup"><span data-stu-id="3daa0-139">description</span></span>|<span data-ttu-id="3daa0-140">String</span><span class="sxs-lookup"><span data-stu-id="3daa0-140">String</span></span>|<span data-ttu-id="3daa0-141">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="3daa0-141">Description of the profile</span></span>|
|<span data-ttu-id="3daa0-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="3daa0-142">requiresUserAuthentication</span></span>|<span data-ttu-id="3daa0-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="3daa0-143">Boolean</span></span>|<span data-ttu-id="3daa0-144">プロファイルにユーザー認証が必要なかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="3daa0-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="3daa0-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="3daa0-145">configurationEndpointUrl</span></span>|<span data-ttu-id="3daa0-146">String</span><span class="sxs-lookup"><span data-stu-id="3daa0-146">String</span></span>|<span data-ttu-id="3daa0-147">登録に使用するエンドポイントの url を構成</span><span class="sxs-lookup"><span data-stu-id="3daa0-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="3daa0-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="3daa0-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="3daa0-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="3daa0-149">Boolean</span></span>|<span data-ttu-id="3daa0-150">アップルらくらく企業ポータルではなくを使用して認証することを示します。</span><span class="sxs-lookup"><span data-stu-id="3daa0-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="3daa0-151">応答</span><span class="sxs-lookup"><span data-stu-id="3daa0-151">Response</span></span>
<span data-ttu-id="3daa0-152">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3daa0-152">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3daa0-153">例</span><span class="sxs-lookup"><span data-stu-id="3daa0-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="3daa0-154">要求</span><span class="sxs-lookup"><span data-stu-id="3daa0-154">Request</span></span>
<span data-ttu-id="3daa0-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3daa0-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```

### <a name="response"></a><span data-ttu-id="3daa0-156">応答</span><span class="sxs-lookup"><span data-stu-id="3daa0-156">Response</span></span>
<span data-ttu-id="3daa0-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3daa0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





