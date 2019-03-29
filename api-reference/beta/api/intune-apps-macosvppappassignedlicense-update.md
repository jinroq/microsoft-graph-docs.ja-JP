---
title: macOsVppAppAssignedLicense の更新
description: macOsVppAppAssignedLicense オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0481a40d07038c98778c1968347a2c6886fe3a86
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979656"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="cf51b-103">macOsVppAppAssignedLicense の更新</span><span class="sxs-lookup"><span data-stu-id="cf51b-103">Update macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="cf51b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf51b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf51b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf51b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf51b-106">[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cf51b-106">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf51b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="cf51b-107">Prerequisites</span></span>
<span data-ttu-id="cf51b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf51b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf51b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf51b-110">Permission type</span></span>|<span data-ttu-id="cf51b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cf51b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf51b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cf51b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf51b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf51b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cf51b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf51b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf51b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf51b-115">Not supported.</span></span>|
|<span data-ttu-id="cf51b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf51b-116">Application</span></span>|<span data-ttu-id="cf51b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf51b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf51b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf51b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="cf51b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf51b-119">Request headers</span></span>
|<span data-ttu-id="cf51b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf51b-120">Header</span></span>|<span data-ttu-id="cf51b-121">値</span><span class="sxs-lookup"><span data-stu-id="cf51b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf51b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf51b-122">Authorization</span></span>|<span data-ttu-id="cf51b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf51b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf51b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="cf51b-124">Accept</span></span>|<span data-ttu-id="cf51b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cf51b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf51b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cf51b-126">Request body</span></span>
<span data-ttu-id="cf51b-127">要求本文で、 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cf51b-127">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="cf51b-128">次の表に、 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cf51b-128">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="cf51b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf51b-129">Property</span></span>|<span data-ttu-id="cf51b-130">型</span><span class="sxs-lookup"><span data-stu-id="cf51b-130">Type</span></span>|<span data-ttu-id="cf51b-131">説明</span><span class="sxs-lookup"><span data-stu-id="cf51b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf51b-132">id</span><span class="sxs-lookup"><span data-stu-id="cf51b-132">id</span></span>|<span data-ttu-id="cf51b-133">String</span><span class="sxs-lookup"><span data-stu-id="cf51b-133">String</span></span>|<span data-ttu-id="cf51b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cf51b-134">Key of the entity.</span></span>|
|<span data-ttu-id="cf51b-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="cf51b-135">userEmailAddress</span></span>|<span data-ttu-id="cf51b-136">String</span><span class="sxs-lookup"><span data-stu-id="cf51b-136">String</span></span>|<span data-ttu-id="cf51b-137">ユーザーの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="cf51b-137">The user email address.</span></span>|
|<span data-ttu-id="cf51b-138">userId</span><span class="sxs-lookup"><span data-stu-id="cf51b-138">userId</span></span>|<span data-ttu-id="cf51b-139">String</span><span class="sxs-lookup"><span data-stu-id="cf51b-139">String</span></span>|<span data-ttu-id="cf51b-140">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="cf51b-140">The user ID.</span></span>|
|<span data-ttu-id="cf51b-141">userName</span><span class="sxs-lookup"><span data-stu-id="cf51b-141">userName</span></span>|<span data-ttu-id="cf51b-142">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="cf51b-142">String</span></span>|<span data-ttu-id="cf51b-143">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="cf51b-143">The user name.</span></span>|
|<span data-ttu-id="cf51b-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cf51b-144">userPrincipalName</span></span>|<span data-ttu-id="cf51b-145">String</span><span class="sxs-lookup"><span data-stu-id="cf51b-145">String</span></span>|<span data-ttu-id="cf51b-146">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="cf51b-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="cf51b-147">応答</span><span class="sxs-lookup"><span data-stu-id="cf51b-147">Response</span></span>
<span data-ttu-id="cf51b-148">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cf51b-148">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf51b-149">例</span><span class="sxs-lookup"><span data-stu-id="cf51b-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf51b-150">要求</span><span class="sxs-lookup"><span data-stu-id="cf51b-150">Request</span></span>
<span data-ttu-id="cf51b-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cf51b-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cf51b-152">応答</span><span class="sxs-lookup"><span data-stu-id="cf51b-152">Response</span></span>
<span data-ttu-id="cf51b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cf51b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




