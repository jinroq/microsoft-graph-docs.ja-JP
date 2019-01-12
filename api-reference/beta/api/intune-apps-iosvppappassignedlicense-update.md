---
title: IosVppAppAssignedLicense を更新します。
description: IosVppAppAssignedLicense オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 86b618275d1312953d14367d23bbde99aee0cff4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969073"
---
# <a name="update-iosvppappassignedlicense"></a><span data-ttu-id="aa17b-103">IosVppAppAssignedLicense を更新します。</span><span class="sxs-lookup"><span data-stu-id="aa17b-103">Update iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="aa17b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aa17b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa17b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa17b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa17b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aa17b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa17b-107">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aa17b-107">Update the properties of a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aa17b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="aa17b-108">Prerequisites</span></span>
<span data-ttu-id="aa17b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aa17b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa17b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aa17b-111">Permission type</span></span>|<span data-ttu-id="aa17b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aa17b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa17b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aa17b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa17b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa17b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aa17b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aa17b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa17b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa17b-116">Not supported.</span></span>|
|<span data-ttu-id="aa17b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aa17b-117">Application</span></span>|<span data-ttu-id="aa17b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa17b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa17b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aa17b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="aa17b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aa17b-120">Request headers</span></span>
|<span data-ttu-id="aa17b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aa17b-121">Header</span></span>|<span data-ttu-id="aa17b-122">値</span><span class="sxs-lookup"><span data-stu-id="aa17b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa17b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa17b-123">Authorization</span></span>|<span data-ttu-id="aa17b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="aa17b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa17b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aa17b-125">Accept</span></span>|<span data-ttu-id="aa17b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa17b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa17b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="aa17b-127">Request body</span></span>
<span data-ttu-id="aa17b-128">要求の本文に[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="aa17b-128">In the request body, supply a JSON representation for the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="aa17b-129">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="aa17b-129">The following table shows the properties that are required when you create the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="aa17b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa17b-130">Property</span></span>|<span data-ttu-id="aa17b-131">種類</span><span class="sxs-lookup"><span data-stu-id="aa17b-131">Type</span></span>|<span data-ttu-id="aa17b-132">説明</span><span class="sxs-lookup"><span data-stu-id="aa17b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa17b-133">ID</span><span class="sxs-lookup"><span data-stu-id="aa17b-133">id</span></span>|<span data-ttu-id="aa17b-134">String</span><span class="sxs-lookup"><span data-stu-id="aa17b-134">String</span></span>|<span data-ttu-id="aa17b-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="aa17b-135">Key of the entity.</span></span>|
|<span data-ttu-id="aa17b-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="aa17b-136">userEmailAddress</span></span>|<span data-ttu-id="aa17b-137">String</span><span class="sxs-lookup"><span data-stu-id="aa17b-137">String</span></span>|<span data-ttu-id="aa17b-138">ユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="aa17b-138">The user email address.</span></span>|
|<span data-ttu-id="aa17b-139">userId</span><span class="sxs-lookup"><span data-stu-id="aa17b-139">userId</span></span>|<span data-ttu-id="aa17b-140">String</span><span class="sxs-lookup"><span data-stu-id="aa17b-140">String</span></span>|<span data-ttu-id="aa17b-141">ユーザー id。</span><span class="sxs-lookup"><span data-stu-id="aa17b-141">The user ID.</span></span>|
|<span data-ttu-id="aa17b-142">userName</span><span class="sxs-lookup"><span data-stu-id="aa17b-142">userName</span></span>|<span data-ttu-id="aa17b-143">String</span><span class="sxs-lookup"><span data-stu-id="aa17b-143">String</span></span>|<span data-ttu-id="aa17b-144">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="aa17b-144">The user name.</span></span>|
|<span data-ttu-id="aa17b-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aa17b-145">userPrincipalName</span></span>|<span data-ttu-id="aa17b-146">String</span><span class="sxs-lookup"><span data-stu-id="aa17b-146">String</span></span>|<span data-ttu-id="aa17b-147">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="aa17b-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="aa17b-148">応答</span><span class="sxs-lookup"><span data-stu-id="aa17b-148">Response</span></span>
<span data-ttu-id="aa17b-149">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="aa17b-149">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa17b-150">例</span><span class="sxs-lookup"><span data-stu-id="aa17b-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa17b-151">要求</span><span class="sxs-lookup"><span data-stu-id="aa17b-151">Request</span></span>
<span data-ttu-id="aa17b-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aa17b-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 171

{
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="aa17b-153">応答</span><span class="sxs-lookup"><span data-stu-id="aa17b-153">Response</span></span>
<span data-ttu-id="aa17b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa17b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





