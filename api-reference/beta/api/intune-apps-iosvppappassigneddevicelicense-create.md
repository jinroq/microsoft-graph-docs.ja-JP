---
title: iosVppAppAssignedDeviceLicense を作成する
description: 新しい iosVppAppAssignedDeviceLicense オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ced922ee489e1f17f6b33df4a2807fee776fe0ff
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771251"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="75c32-103">iosVppAppAssignedDeviceLicense を作成する</span><span class="sxs-lookup"><span data-stu-id="75c32-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="75c32-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75c32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75c32-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="75c32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75c32-106">新しい[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="75c32-106">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75c32-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="75c32-107">Prerequisites</span></span>
<span data-ttu-id="75c32-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75c32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75c32-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="75c32-110">Permission type</span></span>|<span data-ttu-id="75c32-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="75c32-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75c32-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="75c32-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75c32-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75c32-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="75c32-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="75c32-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75c32-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75c32-115">Not supported.</span></span>|
|<span data-ttu-id="75c32-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="75c32-116">Application</span></span>|<span data-ttu-id="75c32-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75c32-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75c32-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="75c32-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="75c32-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75c32-119">Request headers</span></span>
|<span data-ttu-id="75c32-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75c32-120">Header</span></span>|<span data-ttu-id="75c32-121">値</span><span class="sxs-lookup"><span data-stu-id="75c32-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75c32-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75c32-122">Authorization</span></span>|<span data-ttu-id="75c32-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="75c32-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75c32-124">承諾</span><span class="sxs-lookup"><span data-stu-id="75c32-124">Accept</span></span>|<span data-ttu-id="75c32-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75c32-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75c32-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="75c32-126">Request body</span></span>
<span data-ttu-id="75c32-127">要求本文で、iosVppAppAssignedDeviceLicense オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="75c32-127">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="75c32-128">次の表に、iosVppAppAssignedDeviceLicense の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="75c32-128">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="75c32-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75c32-129">Property</span></span>|<span data-ttu-id="75c32-130">型</span><span class="sxs-lookup"><span data-stu-id="75c32-130">Type</span></span>|<span data-ttu-id="75c32-131">説明</span><span class="sxs-lookup"><span data-stu-id="75c32-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75c32-132">id</span><span class="sxs-lookup"><span data-stu-id="75c32-132">id</span></span>|<span data-ttu-id="75c32-133">String</span><span class="sxs-lookup"><span data-stu-id="75c32-133">String</span></span>|<span data-ttu-id="75c32-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="75c32-134">Key of the entity.</span></span> <span data-ttu-id="75c32-135">[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="75c32-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="75c32-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="75c32-136">userEmailAddress</span></span>|<span data-ttu-id="75c32-137">文字列</span><span class="sxs-lookup"><span data-stu-id="75c32-137">String</span></span>|<span data-ttu-id="75c32-138">ユーザーの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="75c32-138">The user email address.</span></span> <span data-ttu-id="75c32-139">[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="75c32-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="75c32-140">userId</span><span class="sxs-lookup"><span data-stu-id="75c32-140">userId</span></span>|<span data-ttu-id="75c32-141">String</span><span class="sxs-lookup"><span data-stu-id="75c32-141">String</span></span>|<span data-ttu-id="75c32-142">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="75c32-142">The user ID.</span></span> <span data-ttu-id="75c32-143">[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="75c32-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="75c32-144">userName</span><span class="sxs-lookup"><span data-stu-id="75c32-144">userName</span></span>|<span data-ttu-id="75c32-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="75c32-145">String</span></span>|<span data-ttu-id="75c32-146">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="75c32-146">The user name.</span></span> <span data-ttu-id="75c32-147">[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="75c32-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="75c32-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="75c32-148">userPrincipalName</span></span>|<span data-ttu-id="75c32-149">String</span><span class="sxs-lookup"><span data-stu-id="75c32-149">String</span></span>|<span data-ttu-id="75c32-150">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="75c32-150">The user principal name.</span></span> <span data-ttu-id="75c32-151">[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="75c32-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="75c32-152">manageddeviceid</span><span class="sxs-lookup"><span data-stu-id="75c32-152">managedDeviceId</span></span>|<span data-ttu-id="75c32-153">文字列</span><span class="sxs-lookup"><span data-stu-id="75c32-153">String</span></span>|<span data-ttu-id="75c32-154">管理されているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="75c32-154">The managed device ID.</span></span>|
|<span data-ttu-id="75c32-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="75c32-155">deviceName</span></span>|<span data-ttu-id="75c32-156">文字列</span><span class="sxs-lookup"><span data-stu-id="75c32-156">String</span></span>|<span data-ttu-id="75c32-157">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="75c32-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="75c32-158">応答</span><span class="sxs-lookup"><span data-stu-id="75c32-158">Response</span></span>
<span data-ttu-id="75c32-159">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="75c32-159">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75c32-160">例</span><span class="sxs-lookup"><span data-stu-id="75c32-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="75c32-161">要求</span><span class="sxs-lookup"><span data-stu-id="75c32-161">Request</span></span>
<span data-ttu-id="75c32-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="75c32-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75c32-163">応答</span><span class="sxs-lookup"><span data-stu-id="75c32-163">Response</span></span>
<span data-ttu-id="75c32-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="75c32-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





