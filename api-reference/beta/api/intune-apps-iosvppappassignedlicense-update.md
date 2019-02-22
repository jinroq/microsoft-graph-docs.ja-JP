---
title: iosVppAppAssignedLicense の更新
description: iosVppAppAssignedLicense オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d2003ea2c6bbd2a38e3d766de84ba7d224864dd8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169889"
---
# <a name="update-iosvppappassignedlicense"></a><span data-ttu-id="b381e-103">iosVppAppAssignedLicense の更新</span><span class="sxs-lookup"><span data-stu-id="b381e-103">Update iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="b381e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b381e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b381e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b381e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b381e-106">[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b381e-106">Update the properties of a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b381e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b381e-107">Prerequisites</span></span>
<span data-ttu-id="b381e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b381e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b381e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b381e-110">Permission type</span></span>|<span data-ttu-id="b381e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b381e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b381e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b381e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b381e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b381e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b381e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b381e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b381e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b381e-115">Not supported.</span></span>|
|<span data-ttu-id="b381e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b381e-116">Application</span></span>|<span data-ttu-id="b381e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b381e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b381e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b381e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="b381e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b381e-119">Request headers</span></span>
|<span data-ttu-id="b381e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b381e-120">Header</span></span>|<span data-ttu-id="b381e-121">値</span><span class="sxs-lookup"><span data-stu-id="b381e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b381e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b381e-122">Authorization</span></span>|<span data-ttu-id="b381e-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b381e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b381e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b381e-124">Accept</span></span>|<span data-ttu-id="b381e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b381e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b381e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b381e-126">Request body</span></span>
<span data-ttu-id="b381e-127">要求本文で、 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b381e-127">In the request body, supply a JSON representation for the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="b381e-128">次の表に、 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b381e-128">The following table shows the properties that are required when you create the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="b381e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b381e-129">Property</span></span>|<span data-ttu-id="b381e-130">型</span><span class="sxs-lookup"><span data-stu-id="b381e-130">Type</span></span>|<span data-ttu-id="b381e-131">説明</span><span class="sxs-lookup"><span data-stu-id="b381e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b381e-132">id</span><span class="sxs-lookup"><span data-stu-id="b381e-132">id</span></span>|<span data-ttu-id="b381e-133">String</span><span class="sxs-lookup"><span data-stu-id="b381e-133">String</span></span>|<span data-ttu-id="b381e-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b381e-134">Key of the entity.</span></span>|
|<span data-ttu-id="b381e-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="b381e-135">userEmailAddress</span></span>|<span data-ttu-id="b381e-136">String</span><span class="sxs-lookup"><span data-stu-id="b381e-136">String</span></span>|<span data-ttu-id="b381e-137">ユーザーの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="b381e-137">The user email address.</span></span>|
|<span data-ttu-id="b381e-138">userId</span><span class="sxs-lookup"><span data-stu-id="b381e-138">userId</span></span>|<span data-ttu-id="b381e-139">String</span><span class="sxs-lookup"><span data-stu-id="b381e-139">String</span></span>|<span data-ttu-id="b381e-140">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="b381e-140">The user ID.</span></span>|
|<span data-ttu-id="b381e-141">userName</span><span class="sxs-lookup"><span data-stu-id="b381e-141">userName</span></span>|<span data-ttu-id="b381e-142">String</span><span class="sxs-lookup"><span data-stu-id="b381e-142">String</span></span>|<span data-ttu-id="b381e-143">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="b381e-143">The user name.</span></span>|
|<span data-ttu-id="b381e-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b381e-144">userPrincipalName</span></span>|<span data-ttu-id="b381e-145">String</span><span class="sxs-lookup"><span data-stu-id="b381e-145">String</span></span>|<span data-ttu-id="b381e-146">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="b381e-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="b381e-147">応答</span><span class="sxs-lookup"><span data-stu-id="b381e-147">Response</span></span>
<span data-ttu-id="b381e-148">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b381e-148">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b381e-149">例</span><span class="sxs-lookup"><span data-stu-id="b381e-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="b381e-150">要求</span><span class="sxs-lookup"><span data-stu-id="b381e-150">Request</span></span>
<span data-ttu-id="b381e-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b381e-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 234

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="b381e-152">応答</span><span class="sxs-lookup"><span data-stu-id="b381e-152">Response</span></span>
<span data-ttu-id="b381e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b381e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 283

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




