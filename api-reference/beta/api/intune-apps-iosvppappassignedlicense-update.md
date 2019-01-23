---
title: IosVppAppAssignedLicense を更新します。
description: IosVppAppAssignedLicense オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3946ee39c8be93a7c0323da868a65f76d54fc3c2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397548"
---
# <a name="update-iosvppappassignedlicense"></a><span data-ttu-id="f322b-103">IosVppAppAssignedLicense を更新します。</span><span class="sxs-lookup"><span data-stu-id="f322b-103">Update iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="f322b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f322b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f322b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f322b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f322b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f322b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f322b-107">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f322b-107">Update the properties of a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f322b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f322b-108">Prerequisites</span></span>
<span data-ttu-id="f322b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f322b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f322b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f322b-111">Permission type</span></span>|<span data-ttu-id="f322b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f322b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f322b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f322b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f322b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f322b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f322b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f322b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f322b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f322b-116">Not supported.</span></span>|
|<span data-ttu-id="f322b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f322b-117">Application</span></span>|<span data-ttu-id="f322b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f322b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f322b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f322b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="f322b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f322b-120">Request headers</span></span>
|<span data-ttu-id="f322b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f322b-121">Header</span></span>|<span data-ttu-id="f322b-122">値</span><span class="sxs-lookup"><span data-stu-id="f322b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f322b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f322b-123">Authorization</span></span>|<span data-ttu-id="f322b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f322b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f322b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f322b-125">Accept</span></span>|<span data-ttu-id="f322b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f322b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f322b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f322b-127">Request body</span></span>
<span data-ttu-id="f322b-128">要求の本文に[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="f322b-128">In the request body, supply a JSON representation for the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="f322b-129">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f322b-129">The following table shows the properties that are required when you create the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="f322b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f322b-130">Property</span></span>|<span data-ttu-id="f322b-131">型</span><span class="sxs-lookup"><span data-stu-id="f322b-131">Type</span></span>|<span data-ttu-id="f322b-132">説明</span><span class="sxs-lookup"><span data-stu-id="f322b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f322b-133">id</span><span class="sxs-lookup"><span data-stu-id="f322b-133">id</span></span>|<span data-ttu-id="f322b-134">String</span><span class="sxs-lookup"><span data-stu-id="f322b-134">String</span></span>|<span data-ttu-id="f322b-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f322b-135">Key of the entity.</span></span>|
|<span data-ttu-id="f322b-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="f322b-136">userEmailAddress</span></span>|<span data-ttu-id="f322b-137">String</span><span class="sxs-lookup"><span data-stu-id="f322b-137">String</span></span>|<span data-ttu-id="f322b-138">ユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="f322b-138">The user email address.</span></span>|
|<span data-ttu-id="f322b-139">userId</span><span class="sxs-lookup"><span data-stu-id="f322b-139">userId</span></span>|<span data-ttu-id="f322b-140">String</span><span class="sxs-lookup"><span data-stu-id="f322b-140">String</span></span>|<span data-ttu-id="f322b-141">ユーザー id。</span><span class="sxs-lookup"><span data-stu-id="f322b-141">The user ID.</span></span>|
|<span data-ttu-id="f322b-142">userName</span><span class="sxs-lookup"><span data-stu-id="f322b-142">userName</span></span>|<span data-ttu-id="f322b-143">String</span><span class="sxs-lookup"><span data-stu-id="f322b-143">String</span></span>|<span data-ttu-id="f322b-144">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="f322b-144">The user name.</span></span>|
|<span data-ttu-id="f322b-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f322b-145">userPrincipalName</span></span>|<span data-ttu-id="f322b-146">String</span><span class="sxs-lookup"><span data-stu-id="f322b-146">String</span></span>|<span data-ttu-id="f322b-147">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="f322b-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="f322b-148">応答</span><span class="sxs-lookup"><span data-stu-id="f322b-148">Response</span></span>
<span data-ttu-id="f322b-149">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f322b-149">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f322b-150">例</span><span class="sxs-lookup"><span data-stu-id="f322b-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f322b-151">要求</span><span class="sxs-lookup"><span data-stu-id="f322b-151">Request</span></span>
<span data-ttu-id="f322b-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f322b-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f322b-153">応答</span><span class="sxs-lookup"><span data-stu-id="f322b-153">Response</span></span>
<span data-ttu-id="f322b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f322b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




