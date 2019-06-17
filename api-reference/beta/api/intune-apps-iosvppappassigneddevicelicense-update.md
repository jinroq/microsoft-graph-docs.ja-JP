---
title: IosVppAppAssignedDeviceLicense の更新
description: IosVppAppAssignedDeviceLicense オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 716ac5aa2e4f5f2a9412767b446b12a86815e736
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975519"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="887c1-103">IosVppAppAssignedDeviceLicense の更新</span><span class="sxs-lookup"><span data-stu-id="887c1-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="887c1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="887c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="887c1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="887c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="887c1-106">[IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="887c1-106">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="887c1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="887c1-107">Prerequisites</span></span>
<span data-ttu-id="887c1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="887c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="887c1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="887c1-110">Permission type</span></span>|<span data-ttu-id="887c1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="887c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="887c1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="887c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="887c1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="887c1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="887c1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="887c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="887c1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="887c1-115">Not supported.</span></span>|
|<span data-ttu-id="887c1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="887c1-116">Application</span></span>|<span data-ttu-id="887c1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="887c1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="887c1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="887c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="887c1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="887c1-119">Request headers</span></span>
|<span data-ttu-id="887c1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="887c1-120">Header</span></span>|<span data-ttu-id="887c1-121">値</span><span class="sxs-lookup"><span data-stu-id="887c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="887c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="887c1-122">Authorization</span></span>|<span data-ttu-id="887c1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="887c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="887c1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="887c1-124">Accept</span></span>|<span data-ttu-id="887c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="887c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="887c1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="887c1-126">Request body</span></span>
<span data-ttu-id="887c1-127">要求本文で、 [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="887c1-127">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="887c1-128">次の表に、 [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="887c1-128">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="887c1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="887c1-129">Property</span></span>|<span data-ttu-id="887c1-130">型</span><span class="sxs-lookup"><span data-stu-id="887c1-130">Type</span></span>|<span data-ttu-id="887c1-131">説明</span><span class="sxs-lookup"><span data-stu-id="887c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="887c1-132">id</span><span class="sxs-lookup"><span data-stu-id="887c1-132">id</span></span>|<span data-ttu-id="887c1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="887c1-133">String</span></span>|<span data-ttu-id="887c1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="887c1-134">Key of the entity.</span></span> <span data-ttu-id="887c1-135">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="887c1-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="887c1-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="887c1-136">userEmailAddress</span></span>|<span data-ttu-id="887c1-137">String</span><span class="sxs-lookup"><span data-stu-id="887c1-137">String</span></span>|<span data-ttu-id="887c1-138">ユーザーの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="887c1-138">The user email address.</span></span> <span data-ttu-id="887c1-139">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="887c1-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="887c1-140">userId</span><span class="sxs-lookup"><span data-stu-id="887c1-140">userId</span></span>|<span data-ttu-id="887c1-141">String</span><span class="sxs-lookup"><span data-stu-id="887c1-141">String</span></span>|<span data-ttu-id="887c1-142">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="887c1-142">The user ID.</span></span> <span data-ttu-id="887c1-143">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="887c1-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="887c1-144">userName</span><span class="sxs-lookup"><span data-stu-id="887c1-144">userName</span></span>|<span data-ttu-id="887c1-145">String</span><span class="sxs-lookup"><span data-stu-id="887c1-145">String</span></span>|<span data-ttu-id="887c1-146">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="887c1-146">The user name.</span></span> <span data-ttu-id="887c1-147">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="887c1-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="887c1-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="887c1-148">userPrincipalName</span></span>|<span data-ttu-id="887c1-149">String</span><span class="sxs-lookup"><span data-stu-id="887c1-149">String</span></span>|<span data-ttu-id="887c1-150">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="887c1-150">The user principal name.</span></span> <span data-ttu-id="887c1-151">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="887c1-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="887c1-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="887c1-152">managedDeviceId</span></span>|<span data-ttu-id="887c1-153">String</span><span class="sxs-lookup"><span data-stu-id="887c1-153">String</span></span>|<span data-ttu-id="887c1-154">管理されているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="887c1-154">The managed device ID.</span></span>|
|<span data-ttu-id="887c1-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="887c1-155">deviceName</span></span>|<span data-ttu-id="887c1-156">String</span><span class="sxs-lookup"><span data-stu-id="887c1-156">String</span></span>|<span data-ttu-id="887c1-157">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="887c1-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="887c1-158">応答</span><span class="sxs-lookup"><span data-stu-id="887c1-158">Response</span></span>
<span data-ttu-id="887c1-159">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="887c1-159">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="887c1-160">例</span><span class="sxs-lookup"><span data-stu-id="887c1-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="887c1-161">要求</span><span class="sxs-lookup"><span data-stu-id="887c1-161">Request</span></span>
<span data-ttu-id="887c1-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="887c1-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
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

### <a name="response"></a><span data-ttu-id="887c1-163">応答</span><span class="sxs-lookup"><span data-stu-id="887c1-163">Response</span></span>
<span data-ttu-id="887c1-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="887c1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





