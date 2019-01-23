---
title: IosVppAppAssignedUserLicense を作成します。
description: 新しい iosVppAppAssignedUserLicense オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1da8eebaa02564b4407face3fd866438d29304d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417897"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="04f16-103">IosVppAppAssignedUserLicense を作成します。</span><span class="sxs-lookup"><span data-stu-id="04f16-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="04f16-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04f16-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04f16-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04f16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04f16-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="04f16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04f16-107">新しい[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="04f16-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04f16-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="04f16-108">Prerequisites</span></span>
<span data-ttu-id="04f16-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04f16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="04f16-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04f16-111">Permission type</span></span>|<span data-ttu-id="04f16-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="04f16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04f16-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04f16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04f16-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04f16-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04f16-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04f16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04f16-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04f16-116">Not supported.</span></span>|
|<span data-ttu-id="04f16-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04f16-117">Application</span></span>|<span data-ttu-id="04f16-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04f16-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04f16-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04f16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="04f16-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04f16-120">Request headers</span></span>
|<span data-ttu-id="04f16-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04f16-121">Header</span></span>|<span data-ttu-id="04f16-122">値</span><span class="sxs-lookup"><span data-stu-id="04f16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04f16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04f16-123">Authorization</span></span>|<span data-ttu-id="04f16-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="04f16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04f16-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04f16-125">Accept</span></span>|<span data-ttu-id="04f16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04f16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04f16-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="04f16-127">Request body</span></span>
<span data-ttu-id="04f16-128">要求の本文に iosVppAppAssignedUserLicense オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="04f16-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="04f16-129">次の表は、iosVppAppAssignedUserLicense を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="04f16-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="04f16-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04f16-130">Property</span></span>|<span data-ttu-id="04f16-131">型</span><span class="sxs-lookup"><span data-stu-id="04f16-131">Type</span></span>|<span data-ttu-id="04f16-132">説明</span><span class="sxs-lookup"><span data-stu-id="04f16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04f16-133">id</span><span class="sxs-lookup"><span data-stu-id="04f16-133">id</span></span>|<span data-ttu-id="04f16-134">String</span><span class="sxs-lookup"><span data-stu-id="04f16-134">String</span></span>|<span data-ttu-id="04f16-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="04f16-135">Key of the entity.</span></span> <span data-ttu-id="04f16-136">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="04f16-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="04f16-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="04f16-137">userEmailAddress</span></span>|<span data-ttu-id="04f16-138">String</span><span class="sxs-lookup"><span data-stu-id="04f16-138">String</span></span>|<span data-ttu-id="04f16-139">ユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="04f16-139">The user email address.</span></span> <span data-ttu-id="04f16-140">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="04f16-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="04f16-141">userId</span><span class="sxs-lookup"><span data-stu-id="04f16-141">userId</span></span>|<span data-ttu-id="04f16-142">String</span><span class="sxs-lookup"><span data-stu-id="04f16-142">String</span></span>|<span data-ttu-id="04f16-143">ユーザー id。</span><span class="sxs-lookup"><span data-stu-id="04f16-143">The user ID.</span></span> <span data-ttu-id="04f16-144">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="04f16-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="04f16-145">userName</span><span class="sxs-lookup"><span data-stu-id="04f16-145">userName</span></span>|<span data-ttu-id="04f16-146">String</span><span class="sxs-lookup"><span data-stu-id="04f16-146">String</span></span>|<span data-ttu-id="04f16-147">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="04f16-147">The user name.</span></span> <span data-ttu-id="04f16-148">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="04f16-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="04f16-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="04f16-149">userPrincipalName</span></span>|<span data-ttu-id="04f16-150">String</span><span class="sxs-lookup"><span data-stu-id="04f16-150">String</span></span>|<span data-ttu-id="04f16-151">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="04f16-151">The user principal name.</span></span> <span data-ttu-id="04f16-152">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="04f16-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="04f16-153">応答</span><span class="sxs-lookup"><span data-stu-id="04f16-153">Response</span></span>
<span data-ttu-id="04f16-154">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="04f16-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04f16-155">例</span><span class="sxs-lookup"><span data-stu-id="04f16-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="04f16-156">要求</span><span class="sxs-lookup"><span data-stu-id="04f16-156">Request</span></span>
<span data-ttu-id="04f16-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04f16-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="04f16-158">応答</span><span class="sxs-lookup"><span data-stu-id="04f16-158">Response</span></span>
<span data-ttu-id="04f16-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04f16-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




