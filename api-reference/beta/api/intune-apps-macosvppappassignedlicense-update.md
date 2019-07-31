---
title: MacOsVppAppAssignedLicense の更新
description: MacOsVppAppAssignedLicense オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db54bb8103f309bac27e7b1a4a40808804dcc833
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961904"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="5f320-103">MacOsVppAppAssignedLicense の更新</span><span class="sxs-lookup"><span data-stu-id="5f320-103">Update macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="5f320-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f320-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f320-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5f320-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f320-106">[MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5f320-106">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f320-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5f320-107">Prerequisites</span></span>
<span data-ttu-id="5f320-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f320-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f320-110">Permission type</span></span>|<span data-ttu-id="5f320-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f320-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f320-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f320-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f320-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f320-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5f320-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f320-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f320-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f320-115">Not supported.</span></span>|
|<span data-ttu-id="5f320-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f320-116">Application</span></span>|<span data-ttu-id="5f320-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f320-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f320-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f320-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="5f320-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f320-119">Request headers</span></span>
|<span data-ttu-id="5f320-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f320-120">Header</span></span>|<span data-ttu-id="5f320-121">値</span><span class="sxs-lookup"><span data-stu-id="5f320-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f320-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f320-122">Authorization</span></span>|<span data-ttu-id="5f320-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5f320-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f320-124">承諾</span><span class="sxs-lookup"><span data-stu-id="5f320-124">Accept</span></span>|<span data-ttu-id="5f320-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f320-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f320-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f320-126">Request body</span></span>
<span data-ttu-id="5f320-127">要求本文で、 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5f320-127">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="5f320-128">次の表に、 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5f320-128">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="5f320-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f320-129">Property</span></span>|<span data-ttu-id="5f320-130">型</span><span class="sxs-lookup"><span data-stu-id="5f320-130">Type</span></span>|<span data-ttu-id="5f320-131">説明</span><span class="sxs-lookup"><span data-stu-id="5f320-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f320-132">id</span><span class="sxs-lookup"><span data-stu-id="5f320-132">id</span></span>|<span data-ttu-id="5f320-133">文字列</span><span class="sxs-lookup"><span data-stu-id="5f320-133">String</span></span>|<span data-ttu-id="5f320-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5f320-134">Key of the entity.</span></span>|
|<span data-ttu-id="5f320-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="5f320-135">userEmailAddress</span></span>|<span data-ttu-id="5f320-136">String</span><span class="sxs-lookup"><span data-stu-id="5f320-136">String</span></span>|<span data-ttu-id="5f320-137">ユーザーの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="5f320-137">The user email address.</span></span>|
|<span data-ttu-id="5f320-138">userId</span><span class="sxs-lookup"><span data-stu-id="5f320-138">userId</span></span>|<span data-ttu-id="5f320-139">String</span><span class="sxs-lookup"><span data-stu-id="5f320-139">String</span></span>|<span data-ttu-id="5f320-140">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="5f320-140">The user ID.</span></span>|
|<span data-ttu-id="5f320-141">userName</span><span class="sxs-lookup"><span data-stu-id="5f320-141">userName</span></span>|<span data-ttu-id="5f320-142">String</span><span class="sxs-lookup"><span data-stu-id="5f320-142">String</span></span>|<span data-ttu-id="5f320-143">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="5f320-143">The user name.</span></span>|
|<span data-ttu-id="5f320-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5f320-144">userPrincipalName</span></span>|<span data-ttu-id="5f320-145">String</span><span class="sxs-lookup"><span data-stu-id="5f320-145">String</span></span>|<span data-ttu-id="5f320-146">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="5f320-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="5f320-147">応答</span><span class="sxs-lookup"><span data-stu-id="5f320-147">Response</span></span>
<span data-ttu-id="5f320-148">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5f320-148">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f320-149">例</span><span class="sxs-lookup"><span data-stu-id="5f320-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f320-150">要求</span><span class="sxs-lookup"><span data-stu-id="5f320-150">Request</span></span>
<span data-ttu-id="5f320-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5f320-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="5f320-152">応答</span><span class="sxs-lookup"><span data-stu-id="5f320-152">Response</span></span>
<span data-ttu-id="5f320-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5f320-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```





