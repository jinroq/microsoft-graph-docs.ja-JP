---
title: MacOsVppAppAssignedLicense を作成する
description: 新しい macOsVppAppAssignedLicense オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9738b39b3d30c5c246fdfd77788187a7dc46a47a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935826"
---
# <a name="create-macosvppappassignedlicense"></a><span data-ttu-id="8df99-103">MacOsVppAppAssignedLicense を作成する</span><span class="sxs-lookup"><span data-stu-id="8df99-103">Create macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="8df99-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8df99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8df99-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8df99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8df99-106">新しい[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8df99-106">Create a new [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8df99-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8df99-107">Prerequisites</span></span>
<span data-ttu-id="8df99-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8df99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8df99-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8df99-110">Permission type</span></span>|<span data-ttu-id="8df99-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8df99-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8df99-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8df99-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8df99-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df99-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8df99-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8df99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8df99-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8df99-115">Not supported.</span></span>|
|<span data-ttu-id="8df99-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8df99-116">Application</span></span>|<span data-ttu-id="8df99-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8df99-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8df99-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8df99-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="8df99-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8df99-119">Request headers</span></span>
|<span data-ttu-id="8df99-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8df99-120">Header</span></span>|<span data-ttu-id="8df99-121">値</span><span class="sxs-lookup"><span data-stu-id="8df99-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8df99-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8df99-122">Authorization</span></span>|<span data-ttu-id="8df99-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8df99-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8df99-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8df99-124">Accept</span></span>|<span data-ttu-id="8df99-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8df99-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8df99-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8df99-126">Request body</span></span>
<span data-ttu-id="8df99-127">要求本文で、macOsVppAppAssignedLicense オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8df99-127">In the request body, supply a JSON representation for the macOsVppAppAssignedLicense object.</span></span>

<span data-ttu-id="8df99-128">次の表に、macOsVppAppAssignedLicense の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8df99-128">The following table shows the properties that are required when you create the macOsVppAppAssignedLicense.</span></span>

|<span data-ttu-id="8df99-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8df99-129">Property</span></span>|<span data-ttu-id="8df99-130">型</span><span class="sxs-lookup"><span data-stu-id="8df99-130">Type</span></span>|<span data-ttu-id="8df99-131">説明</span><span class="sxs-lookup"><span data-stu-id="8df99-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8df99-132">id</span><span class="sxs-lookup"><span data-stu-id="8df99-132">id</span></span>|<span data-ttu-id="8df99-133">文字列</span><span class="sxs-lookup"><span data-stu-id="8df99-133">String</span></span>|<span data-ttu-id="8df99-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8df99-134">Key of the entity.</span></span>|
|<span data-ttu-id="8df99-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8df99-135">userEmailAddress</span></span>|<span data-ttu-id="8df99-136">String</span><span class="sxs-lookup"><span data-stu-id="8df99-136">String</span></span>|<span data-ttu-id="8df99-137">ユーザーの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="8df99-137">The user email address.</span></span>|
|<span data-ttu-id="8df99-138">userId</span><span class="sxs-lookup"><span data-stu-id="8df99-138">userId</span></span>|<span data-ttu-id="8df99-139">String</span><span class="sxs-lookup"><span data-stu-id="8df99-139">String</span></span>|<span data-ttu-id="8df99-140">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="8df99-140">The user ID.</span></span>|
|<span data-ttu-id="8df99-141">userName</span><span class="sxs-lookup"><span data-stu-id="8df99-141">userName</span></span>|<span data-ttu-id="8df99-142">String</span><span class="sxs-lookup"><span data-stu-id="8df99-142">String</span></span>|<span data-ttu-id="8df99-143">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="8df99-143">The user name.</span></span>|
|<span data-ttu-id="8df99-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8df99-144">userPrincipalName</span></span>|<span data-ttu-id="8df99-145">String</span><span class="sxs-lookup"><span data-stu-id="8df99-145">String</span></span>|<span data-ttu-id="8df99-146">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="8df99-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="8df99-147">応答</span><span class="sxs-lookup"><span data-stu-id="8df99-147">Response</span></span>
<span data-ttu-id="8df99-148">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8df99-148">If successful, this method returns a `201 Created` response code and a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8df99-149">例</span><span class="sxs-lookup"><span data-stu-id="8df99-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="8df99-150">要求</span><span class="sxs-lookup"><span data-stu-id="8df99-150">Request</span></span>
<span data-ttu-id="8df99-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8df99-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
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

### <a name="response"></a><span data-ttu-id="8df99-152">応答</span><span class="sxs-lookup"><span data-stu-id="8df99-152">Response</span></span>
<span data-ttu-id="8df99-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8df99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




