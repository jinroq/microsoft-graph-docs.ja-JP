---
title: IosVppAppAssignedLicense を作成します。
description: 新しい iosVppAppAssignedLicense オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65c0b449b1b9add9697d5c1453245efbd1b2e213
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936320"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="978f9-103">IosVppAppAssignedLicense を作成します。</span><span class="sxs-lookup"><span data-stu-id="978f9-103">Create iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="978f9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="978f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="978f9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="978f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="978f9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="978f9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="978f9-107">新しい[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="978f9-107">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="978f9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="978f9-108">Prerequisites</span></span>
<span data-ttu-id="978f9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="978f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="978f9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="978f9-111">Permission type</span></span>|<span data-ttu-id="978f9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="978f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="978f9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="978f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="978f9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="978f9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="978f9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="978f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="978f9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="978f9-116">Not supported.</span></span>|
|<span data-ttu-id="978f9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="978f9-117">Application</span></span>|<span data-ttu-id="978f9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="978f9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="978f9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="978f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="978f9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="978f9-120">Request headers</span></span>
|<span data-ttu-id="978f9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="978f9-121">Header</span></span>|<span data-ttu-id="978f9-122">値</span><span class="sxs-lookup"><span data-stu-id="978f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="978f9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="978f9-123">Authorization</span></span>|<span data-ttu-id="978f9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="978f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="978f9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="978f9-125">Accept</span></span>|<span data-ttu-id="978f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="978f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="978f9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="978f9-127">Request body</span></span>
<span data-ttu-id="978f9-128">要求の本文に iosVppAppAssignedLicense オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="978f9-128">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="978f9-129">次の表は、iosVppAppAssignedLicense を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="978f9-129">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="978f9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="978f9-130">Property</span></span>|<span data-ttu-id="978f9-131">型</span><span class="sxs-lookup"><span data-stu-id="978f9-131">Type</span></span>|<span data-ttu-id="978f9-132">説明</span><span class="sxs-lookup"><span data-stu-id="978f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="978f9-133">ID</span><span class="sxs-lookup"><span data-stu-id="978f9-133">id</span></span>|<span data-ttu-id="978f9-134">String</span><span class="sxs-lookup"><span data-stu-id="978f9-134">String</span></span>|<span data-ttu-id="978f9-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="978f9-135">Key of the entity.</span></span>|
|<span data-ttu-id="978f9-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="978f9-136">userEmailAddress</span></span>|<span data-ttu-id="978f9-137">String</span><span class="sxs-lookup"><span data-stu-id="978f9-137">String</span></span>|<span data-ttu-id="978f9-138">ユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="978f9-138">The user email address.</span></span>|
|<span data-ttu-id="978f9-139">userId</span><span class="sxs-lookup"><span data-stu-id="978f9-139">userId</span></span>|<span data-ttu-id="978f9-140">String</span><span class="sxs-lookup"><span data-stu-id="978f9-140">String</span></span>|<span data-ttu-id="978f9-141">ユーザー id。</span><span class="sxs-lookup"><span data-stu-id="978f9-141">The user ID.</span></span>|
|<span data-ttu-id="978f9-142">userName</span><span class="sxs-lookup"><span data-stu-id="978f9-142">userName</span></span>|<span data-ttu-id="978f9-143">String</span><span class="sxs-lookup"><span data-stu-id="978f9-143">String</span></span>|<span data-ttu-id="978f9-144">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="978f9-144">The user name.</span></span>|
|<span data-ttu-id="978f9-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="978f9-145">userPrincipalName</span></span>|<span data-ttu-id="978f9-146">String</span><span class="sxs-lookup"><span data-stu-id="978f9-146">String</span></span>|<span data-ttu-id="978f9-147">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="978f9-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="978f9-148">応答</span><span class="sxs-lookup"><span data-stu-id="978f9-148">Response</span></span>
<span data-ttu-id="978f9-149">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="978f9-149">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="978f9-150">例</span><span class="sxs-lookup"><span data-stu-id="978f9-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="978f9-151">要求</span><span class="sxs-lookup"><span data-stu-id="978f9-151">Request</span></span>
<span data-ttu-id="978f9-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="978f9-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
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

### <a name="response"></a><span data-ttu-id="978f9-153">応答</span><span class="sxs-lookup"><span data-stu-id="978f9-153">Response</span></span>
<span data-ttu-id="978f9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="978f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





