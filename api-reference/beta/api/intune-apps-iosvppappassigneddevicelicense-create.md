---
title: IosVppAppAssignedDeviceLicense を作成します。
description: 新しい iosVppAppAssignedDeviceLicense オブジェクトを作成します。
ms.openlocfilehash: 968f272fae21ccf78d41b384c34675f6a5d3f4c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072414"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="bcb4b-103">IosVppAppAssignedDeviceLicense を作成します。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="bcb4b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bcb4b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bcb4b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bcb4b-107">新しい[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bcb4b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bcb4b-108">Prerequisites</span></span>
<span data-ttu-id="bcb4b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcb4b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bcb4b-111">Permission type</span></span>|<span data-ttu-id="bcb4b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bcb4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcb4b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bcb4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bcb4b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcb4b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bcb4b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bcb4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcb4b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-116">Not supported.</span></span>|
|<span data-ttu-id="bcb4b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bcb4b-117">Application</span></span>|<span data-ttu-id="bcb4b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcb4b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bcb4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="bcb4b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bcb4b-120">Request headers</span></span>
|<span data-ttu-id="bcb4b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bcb4b-121">Header</span></span>|<span data-ttu-id="bcb4b-122">値</span><span class="sxs-lookup"><span data-stu-id="bcb4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcb4b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcb4b-123">Authorization</span></span>|<span data-ttu-id="bcb4b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcb4b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bcb4b-125">Accept</span></span>|<span data-ttu-id="bcb4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bcb4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcb4b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bcb4b-127">Request body</span></span>
<span data-ttu-id="bcb4b-128">要求の本文に iosVppAppAssignedDeviceLicense オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="bcb4b-129">次の表は、iosVppAppAssignedDeviceLicense を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="bcb4b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcb4b-130">Property</span></span>|<span data-ttu-id="bcb4b-131">型</span><span class="sxs-lookup"><span data-stu-id="bcb4b-131">Type</span></span>|<span data-ttu-id="bcb4b-132">説明</span><span class="sxs-lookup"><span data-stu-id="bcb4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcb4b-133">id</span><span class="sxs-lookup"><span data-stu-id="bcb4b-133">id</span></span>|<span data-ttu-id="bcb4b-134">String</span><span class="sxs-lookup"><span data-stu-id="bcb4b-134">String</span></span>|<span data-ttu-id="bcb4b-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-135">Key of the entity.</span></span> <span data-ttu-id="bcb4b-136">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="bcb4b-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="bcb4b-137">userEmailAddress</span></span>|<span data-ttu-id="bcb4b-138">String</span><span class="sxs-lookup"><span data-stu-id="bcb4b-138">String</span></span>|<span data-ttu-id="bcb4b-139">ユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-139">The user email address.</span></span> <span data-ttu-id="bcb4b-140">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="bcb4b-141">userId</span><span class="sxs-lookup"><span data-stu-id="bcb4b-141">userId</span></span>|<span data-ttu-id="bcb4b-142">String</span><span class="sxs-lookup"><span data-stu-id="bcb4b-142">String</span></span>|<span data-ttu-id="bcb4b-143">ユーザー id。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-143">The user ID.</span></span> <span data-ttu-id="bcb4b-144">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="bcb4b-145">userName</span><span class="sxs-lookup"><span data-stu-id="bcb4b-145">userName</span></span>|<span data-ttu-id="bcb4b-146">String</span><span class="sxs-lookup"><span data-stu-id="bcb4b-146">String</span></span>|<span data-ttu-id="bcb4b-147">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-147">The user name.</span></span> <span data-ttu-id="bcb4b-148">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="bcb4b-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bcb4b-149">userPrincipalName</span></span>|<span data-ttu-id="bcb4b-150">String</span><span class="sxs-lookup"><span data-stu-id="bcb4b-150">String</span></span>|<span data-ttu-id="bcb4b-151">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-151">The user principal name.</span></span> <span data-ttu-id="bcb4b-152">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="bcb4b-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="bcb4b-153">managedDeviceId</span></span>|<span data-ttu-id="bcb4b-154">String</span><span class="sxs-lookup"><span data-stu-id="bcb4b-154">String</span></span>|<span data-ttu-id="bcb4b-155">管理対象デバイスの id。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-155">The managed device ID.</span></span>|
|<span data-ttu-id="bcb4b-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="bcb4b-156">deviceName</span></span>|<span data-ttu-id="bcb4b-157">String</span><span class="sxs-lookup"><span data-stu-id="bcb4b-157">String</span></span>|<span data-ttu-id="bcb4b-158">デバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="bcb4b-159">応答</span><span class="sxs-lookup"><span data-stu-id="bcb4b-159">Response</span></span>
<span data-ttu-id="bcb4b-160">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcb4b-161">例</span><span class="sxs-lookup"><span data-stu-id="bcb4b-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="bcb4b-162">要求</span><span class="sxs-lookup"><span data-stu-id="bcb4b-162">Request</span></span>
<span data-ttu-id="bcb4b-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
Content-type: application/json
Content-length: 327

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="bcb4b-164">応答</span><span class="sxs-lookup"><span data-stu-id="bcb4b-164">Response</span></span>
<span data-ttu-id="bcb4b-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bcb4b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 376

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "id": "bed943d0-43d0-bed9-d043-d9bed043d9be",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```





