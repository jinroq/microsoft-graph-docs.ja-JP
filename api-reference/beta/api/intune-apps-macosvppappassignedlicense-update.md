---
title: MacOsVppAppAssignedLicense を更新します。
description: MacOsVppAppAssignedLicense オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0e3a8a2c54035a29225be547c9971d70fb70f92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431642"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="a12dd-103">MacOsVppAppAssignedLicense を更新します。</span><span class="sxs-lookup"><span data-stu-id="a12dd-103">Update macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="a12dd-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a12dd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a12dd-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a12dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a12dd-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a12dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a12dd-107">[MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a12dd-107">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a12dd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a12dd-108">Prerequisites</span></span>
<span data-ttu-id="a12dd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a12dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a12dd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a12dd-111">Permission type</span></span>|<span data-ttu-id="a12dd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a12dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a12dd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a12dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a12dd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a12dd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a12dd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a12dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a12dd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a12dd-116">Not supported.</span></span>|
|<span data-ttu-id="a12dd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a12dd-117">Application</span></span>|<span data-ttu-id="a12dd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a12dd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a12dd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a12dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="a12dd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a12dd-120">Request headers</span></span>
|<span data-ttu-id="a12dd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a12dd-121">Header</span></span>|<span data-ttu-id="a12dd-122">値</span><span class="sxs-lookup"><span data-stu-id="a12dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a12dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a12dd-123">Authorization</span></span>|<span data-ttu-id="a12dd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a12dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a12dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a12dd-125">Accept</span></span>|<span data-ttu-id="a12dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a12dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a12dd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a12dd-127">Request body</span></span>
<span data-ttu-id="a12dd-128">要求の本文に[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="a12dd-128">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="a12dd-129">[MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="a12dd-129">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="a12dd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a12dd-130">Property</span></span>|<span data-ttu-id="a12dd-131">型</span><span class="sxs-lookup"><span data-stu-id="a12dd-131">Type</span></span>|<span data-ttu-id="a12dd-132">説明</span><span class="sxs-lookup"><span data-stu-id="a12dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a12dd-133">id</span><span class="sxs-lookup"><span data-stu-id="a12dd-133">id</span></span>|<span data-ttu-id="a12dd-134">String</span><span class="sxs-lookup"><span data-stu-id="a12dd-134">String</span></span>|<span data-ttu-id="a12dd-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a12dd-135">Key of the entity.</span></span>|
|<span data-ttu-id="a12dd-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a12dd-136">userEmailAddress</span></span>|<span data-ttu-id="a12dd-137">String</span><span class="sxs-lookup"><span data-stu-id="a12dd-137">String</span></span>|<span data-ttu-id="a12dd-138">ユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="a12dd-138">The user email address.</span></span>|
|<span data-ttu-id="a12dd-139">userId</span><span class="sxs-lookup"><span data-stu-id="a12dd-139">userId</span></span>|<span data-ttu-id="a12dd-140">String</span><span class="sxs-lookup"><span data-stu-id="a12dd-140">String</span></span>|<span data-ttu-id="a12dd-141">ユーザー id。</span><span class="sxs-lookup"><span data-stu-id="a12dd-141">The user ID.</span></span>|
|<span data-ttu-id="a12dd-142">userName</span><span class="sxs-lookup"><span data-stu-id="a12dd-142">userName</span></span>|<span data-ttu-id="a12dd-143">String</span><span class="sxs-lookup"><span data-stu-id="a12dd-143">String</span></span>|<span data-ttu-id="a12dd-144">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="a12dd-144">The user name.</span></span>|
|<span data-ttu-id="a12dd-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a12dd-145">userPrincipalName</span></span>|<span data-ttu-id="a12dd-146">String</span><span class="sxs-lookup"><span data-stu-id="a12dd-146">String</span></span>|<span data-ttu-id="a12dd-147">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="a12dd-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="a12dd-148">応答</span><span class="sxs-lookup"><span data-stu-id="a12dd-148">Response</span></span>
<span data-ttu-id="a12dd-149">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a12dd-149">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a12dd-150">例</span><span class="sxs-lookup"><span data-stu-id="a12dd-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="a12dd-151">要求</span><span class="sxs-lookup"><span data-stu-id="a12dd-151">Request</span></span>
<span data-ttu-id="a12dd-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a12dd-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a12dd-153">応答</span><span class="sxs-lookup"><span data-stu-id="a12dd-153">Response</span></span>
<span data-ttu-id="a12dd-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a12dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




