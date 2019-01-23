---
title: IosVppAppAssignedDeviceLicense を作成します。
description: 新しい iosVppAppAssignedDeviceLicense オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2806e6db550068f46e943f03baca96647176912a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410470"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="0b48f-103">IosVppAppAssignedDeviceLicense を作成します。</span><span class="sxs-lookup"><span data-stu-id="0b48f-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="0b48f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0b48f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0b48f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b48f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b48f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0b48f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b48f-107">新しい[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0b48f-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b48f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0b48f-108">Prerequisites</span></span>
<span data-ttu-id="0b48f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b48f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0b48f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0b48f-111">Permission type</span></span>|<span data-ttu-id="0b48f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0b48f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b48f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0b48f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b48f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b48f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0b48f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b48f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b48f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b48f-116">Not supported.</span></span>|
|<span data-ttu-id="0b48f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0b48f-117">Application</span></span>|<span data-ttu-id="0b48f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b48f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b48f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0b48f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="0b48f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b48f-120">Request headers</span></span>
|<span data-ttu-id="0b48f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b48f-121">Header</span></span>|<span data-ttu-id="0b48f-122">値</span><span class="sxs-lookup"><span data-stu-id="0b48f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b48f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b48f-123">Authorization</span></span>|<span data-ttu-id="0b48f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0b48f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b48f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b48f-125">Accept</span></span>|<span data-ttu-id="0b48f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b48f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b48f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0b48f-127">Request body</span></span>
<span data-ttu-id="0b48f-128">要求の本文に iosVppAppAssignedDeviceLicense オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="0b48f-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="0b48f-129">次の表は、iosVppAppAssignedDeviceLicense を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0b48f-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="0b48f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b48f-130">Property</span></span>|<span data-ttu-id="0b48f-131">型</span><span class="sxs-lookup"><span data-stu-id="0b48f-131">Type</span></span>|<span data-ttu-id="0b48f-132">説明</span><span class="sxs-lookup"><span data-stu-id="0b48f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b48f-133">id</span><span class="sxs-lookup"><span data-stu-id="0b48f-133">id</span></span>|<span data-ttu-id="0b48f-134">String</span><span class="sxs-lookup"><span data-stu-id="0b48f-134">String</span></span>|<span data-ttu-id="0b48f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0b48f-135">Key of the entity.</span></span> <span data-ttu-id="0b48f-136">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0b48f-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0b48f-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0b48f-137">userEmailAddress</span></span>|<span data-ttu-id="0b48f-138">String</span><span class="sxs-lookup"><span data-stu-id="0b48f-138">String</span></span>|<span data-ttu-id="0b48f-139">ユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="0b48f-139">The user email address.</span></span> <span data-ttu-id="0b48f-140">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0b48f-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0b48f-141">userId</span><span class="sxs-lookup"><span data-stu-id="0b48f-141">userId</span></span>|<span data-ttu-id="0b48f-142">String</span><span class="sxs-lookup"><span data-stu-id="0b48f-142">String</span></span>|<span data-ttu-id="0b48f-143">ユーザー id。</span><span class="sxs-lookup"><span data-stu-id="0b48f-143">The user ID.</span></span> <span data-ttu-id="0b48f-144">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0b48f-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0b48f-145">userName</span><span class="sxs-lookup"><span data-stu-id="0b48f-145">userName</span></span>|<span data-ttu-id="0b48f-146">String</span><span class="sxs-lookup"><span data-stu-id="0b48f-146">String</span></span>|<span data-ttu-id="0b48f-147">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="0b48f-147">The user name.</span></span> <span data-ttu-id="0b48f-148">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0b48f-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0b48f-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0b48f-149">userPrincipalName</span></span>|<span data-ttu-id="0b48f-150">String</span><span class="sxs-lookup"><span data-stu-id="0b48f-150">String</span></span>|<span data-ttu-id="0b48f-151">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="0b48f-151">The user principal name.</span></span> <span data-ttu-id="0b48f-152">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="0b48f-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0b48f-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="0b48f-153">managedDeviceId</span></span>|<span data-ttu-id="0b48f-154">String</span><span class="sxs-lookup"><span data-stu-id="0b48f-154">String</span></span>|<span data-ttu-id="0b48f-155">管理対象デバイスの id。</span><span class="sxs-lookup"><span data-stu-id="0b48f-155">The managed device ID.</span></span>|
|<span data-ttu-id="0b48f-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="0b48f-156">deviceName</span></span>|<span data-ttu-id="0b48f-157">String</span><span class="sxs-lookup"><span data-stu-id="0b48f-157">String</span></span>|<span data-ttu-id="0b48f-158">デバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="0b48f-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="0b48f-159">応答</span><span class="sxs-lookup"><span data-stu-id="0b48f-159">Response</span></span>
<span data-ttu-id="0b48f-160">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0b48f-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b48f-161">例</span><span class="sxs-lookup"><span data-stu-id="0b48f-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b48f-162">要求</span><span class="sxs-lookup"><span data-stu-id="0b48f-162">Request</span></span>
<span data-ttu-id="0b48f-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0b48f-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b48f-164">応答</span><span class="sxs-lookup"><span data-stu-id="0b48f-164">Response</span></span>
<span data-ttu-id="0b48f-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0b48f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




