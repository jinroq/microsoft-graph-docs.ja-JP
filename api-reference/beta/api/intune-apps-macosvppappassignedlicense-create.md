---
title: MacOsVppAppAssignedLicense を作成します。
description: 新しい macOsVppAppAssignedLicense オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 07c0bafef2eb86128c8d9bc8cfb071b45bc1e913
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430402"
---
# <a name="create-macosvppappassignedlicense"></a><span data-ttu-id="90996-103">MacOsVppAppAssignedLicense を作成します。</span><span class="sxs-lookup"><span data-stu-id="90996-103">Create macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="90996-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="90996-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="90996-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90996-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90996-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="90996-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90996-107">新しい[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="90996-107">Create a new [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90996-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="90996-108">Prerequisites</span></span>
<span data-ttu-id="90996-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90996-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="90996-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="90996-111">Permission type</span></span>|<span data-ttu-id="90996-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="90996-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90996-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="90996-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90996-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90996-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="90996-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="90996-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90996-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90996-116">Not supported.</span></span>|
|<span data-ttu-id="90996-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="90996-117">Application</span></span>|<span data-ttu-id="90996-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90996-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90996-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="90996-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="90996-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90996-120">Request headers</span></span>
|<span data-ttu-id="90996-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90996-121">Header</span></span>|<span data-ttu-id="90996-122">値</span><span class="sxs-lookup"><span data-stu-id="90996-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90996-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90996-123">Authorization</span></span>|<span data-ttu-id="90996-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="90996-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90996-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90996-125">Accept</span></span>|<span data-ttu-id="90996-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90996-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90996-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="90996-127">Request body</span></span>
<span data-ttu-id="90996-128">要求の本文に macOsVppAppAssignedLicense オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="90996-128">In the request body, supply a JSON representation for the macOsVppAppAssignedLicense object.</span></span>

<span data-ttu-id="90996-129">次の表は、macOsVppAppAssignedLicense を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="90996-129">The following table shows the properties that are required when you create the macOsVppAppAssignedLicense.</span></span>

|<span data-ttu-id="90996-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90996-130">Property</span></span>|<span data-ttu-id="90996-131">型</span><span class="sxs-lookup"><span data-stu-id="90996-131">Type</span></span>|<span data-ttu-id="90996-132">説明</span><span class="sxs-lookup"><span data-stu-id="90996-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90996-133">id</span><span class="sxs-lookup"><span data-stu-id="90996-133">id</span></span>|<span data-ttu-id="90996-134">String</span><span class="sxs-lookup"><span data-stu-id="90996-134">String</span></span>|<span data-ttu-id="90996-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="90996-135">Key of the entity.</span></span>|
|<span data-ttu-id="90996-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="90996-136">userEmailAddress</span></span>|<span data-ttu-id="90996-137">String</span><span class="sxs-lookup"><span data-stu-id="90996-137">String</span></span>|<span data-ttu-id="90996-138">ユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="90996-138">The user email address.</span></span>|
|<span data-ttu-id="90996-139">userId</span><span class="sxs-lookup"><span data-stu-id="90996-139">userId</span></span>|<span data-ttu-id="90996-140">String</span><span class="sxs-lookup"><span data-stu-id="90996-140">String</span></span>|<span data-ttu-id="90996-141">ユーザー id。</span><span class="sxs-lookup"><span data-stu-id="90996-141">The user ID.</span></span>|
|<span data-ttu-id="90996-142">userName</span><span class="sxs-lookup"><span data-stu-id="90996-142">userName</span></span>|<span data-ttu-id="90996-143">String</span><span class="sxs-lookup"><span data-stu-id="90996-143">String</span></span>|<span data-ttu-id="90996-144">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="90996-144">The user name.</span></span>|
|<span data-ttu-id="90996-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="90996-145">userPrincipalName</span></span>|<span data-ttu-id="90996-146">String</span><span class="sxs-lookup"><span data-stu-id="90996-146">String</span></span>|<span data-ttu-id="90996-147">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="90996-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="90996-148">応答</span><span class="sxs-lookup"><span data-stu-id="90996-148">Response</span></span>
<span data-ttu-id="90996-149">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="90996-149">If successful, this method returns a `201 Created` response code and a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90996-150">例</span><span class="sxs-lookup"><span data-stu-id="90996-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="90996-151">要求</span><span class="sxs-lookup"><span data-stu-id="90996-151">Request</span></span>
<span data-ttu-id="90996-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="90996-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="90996-153">応答</span><span class="sxs-lookup"><span data-stu-id="90996-153">Response</span></span>
<span data-ttu-id="90996-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="90996-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




