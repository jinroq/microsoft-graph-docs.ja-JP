---
title: IosVppAppAssignedUserLicense を作成します。
description: 新しい iosVppAppAssignedUserLicense オブジェクトを作成します。
ms.openlocfilehash: 0a4bdad168dcb3baa633cf918ac12b6730e7f61b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072423"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="02488-103">IosVppAppAssignedUserLicense を作成します。</span><span class="sxs-lookup"><span data-stu-id="02488-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="02488-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="02488-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02488-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02488-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02488-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="02488-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02488-107">新しい[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="02488-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02488-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="02488-108">Prerequisites</span></span>
<span data-ttu-id="02488-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02488-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02488-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02488-111">Permission type</span></span>|<span data-ttu-id="02488-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="02488-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02488-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02488-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02488-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02488-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="02488-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02488-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02488-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02488-116">Not supported.</span></span>|
|<span data-ttu-id="02488-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02488-117">Application</span></span>|<span data-ttu-id="02488-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02488-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02488-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02488-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="02488-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02488-120">Request headers</span></span>
|<span data-ttu-id="02488-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02488-121">Header</span></span>|<span data-ttu-id="02488-122">値</span><span class="sxs-lookup"><span data-stu-id="02488-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02488-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02488-123">Authorization</span></span>|<span data-ttu-id="02488-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="02488-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02488-125">Accept</span><span class="sxs-lookup"><span data-stu-id="02488-125">Accept</span></span>|<span data-ttu-id="02488-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02488-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02488-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="02488-127">Request body</span></span>
<span data-ttu-id="02488-128">要求の本文に iosVppAppAssignedUserLicense オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="02488-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="02488-129">次の表は、iosVppAppAssignedUserLicense を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="02488-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="02488-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02488-130">Property</span></span>|<span data-ttu-id="02488-131">型</span><span class="sxs-lookup"><span data-stu-id="02488-131">Type</span></span>|<span data-ttu-id="02488-132">説明</span><span class="sxs-lookup"><span data-stu-id="02488-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02488-133">id</span><span class="sxs-lookup"><span data-stu-id="02488-133">id</span></span>|<span data-ttu-id="02488-134">String</span><span class="sxs-lookup"><span data-stu-id="02488-134">String</span></span>|<span data-ttu-id="02488-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="02488-135">Key of the entity.</span></span> <span data-ttu-id="02488-136">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="02488-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="02488-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="02488-137">userEmailAddress</span></span>|<span data-ttu-id="02488-138">String</span><span class="sxs-lookup"><span data-stu-id="02488-138">String</span></span>|<span data-ttu-id="02488-139">ユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="02488-139">The user email address.</span></span> <span data-ttu-id="02488-140">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="02488-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="02488-141">userId</span><span class="sxs-lookup"><span data-stu-id="02488-141">userId</span></span>|<span data-ttu-id="02488-142">String</span><span class="sxs-lookup"><span data-stu-id="02488-142">String</span></span>|<span data-ttu-id="02488-143">ユーザー id。</span><span class="sxs-lookup"><span data-stu-id="02488-143">The user ID.</span></span> <span data-ttu-id="02488-144">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="02488-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="02488-145">userName</span><span class="sxs-lookup"><span data-stu-id="02488-145">userName</span></span>|<span data-ttu-id="02488-146">String</span><span class="sxs-lookup"><span data-stu-id="02488-146">String</span></span>|<span data-ttu-id="02488-147">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="02488-147">The user name.</span></span> <span data-ttu-id="02488-148">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="02488-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="02488-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="02488-149">userPrincipalName</span></span>|<span data-ttu-id="02488-150">String</span><span class="sxs-lookup"><span data-stu-id="02488-150">String</span></span>|<span data-ttu-id="02488-151">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="02488-151">The user principal name.</span></span> <span data-ttu-id="02488-152">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="02488-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="02488-153">応答</span><span class="sxs-lookup"><span data-stu-id="02488-153">Response</span></span>
<span data-ttu-id="02488-154">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="02488-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02488-155">例</span><span class="sxs-lookup"><span data-stu-id="02488-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="02488-156">要求</span><span class="sxs-lookup"><span data-stu-id="02488-156">Request</span></span>
<span data-ttu-id="02488-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="02488-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="02488-158">応答</span><span class="sxs-lookup"><span data-stu-id="02488-158">Response</span></span>
<span data-ttu-id="02488-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="02488-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





