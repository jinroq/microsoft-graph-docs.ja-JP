---
title: IosVppAppAssignedUserLicense の更新
description: IosVppAppAssignedUserLicense オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aac5234662c55acae0739925674b92c3f2a1a0a4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975365"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="ad92b-103">IosVppAppAssignedUserLicense の更新</span><span class="sxs-lookup"><span data-stu-id="ad92b-103">Update iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="ad92b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad92b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad92b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad92b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad92b-106">[IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ad92b-106">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad92b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ad92b-107">Prerequisites</span></span>
<span data-ttu-id="ad92b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad92b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad92b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad92b-110">Permission type</span></span>|<span data-ttu-id="ad92b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad92b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad92b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad92b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad92b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad92b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ad92b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad92b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad92b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad92b-115">Not supported.</span></span>|
|<span data-ttu-id="ad92b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad92b-116">Application</span></span>|<span data-ttu-id="ad92b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad92b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad92b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad92b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="ad92b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad92b-119">Request headers</span></span>
|<span data-ttu-id="ad92b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad92b-120">Header</span></span>|<span data-ttu-id="ad92b-121">値</span><span class="sxs-lookup"><span data-stu-id="ad92b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad92b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad92b-122">Authorization</span></span>|<span data-ttu-id="ad92b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad92b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad92b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ad92b-124">Accept</span></span>|<span data-ttu-id="ad92b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad92b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad92b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad92b-126">Request body</span></span>
<span data-ttu-id="ad92b-127">要求本文で、 [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad92b-127">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="ad92b-128">次の表に、 [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ad92b-128">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="ad92b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad92b-129">Property</span></span>|<span data-ttu-id="ad92b-130">型</span><span class="sxs-lookup"><span data-stu-id="ad92b-130">Type</span></span>|<span data-ttu-id="ad92b-131">説明</span><span class="sxs-lookup"><span data-stu-id="ad92b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad92b-132">id</span><span class="sxs-lookup"><span data-stu-id="ad92b-132">id</span></span>|<span data-ttu-id="ad92b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ad92b-133">String</span></span>|<span data-ttu-id="ad92b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ad92b-134">Key of the entity.</span></span> <span data-ttu-id="ad92b-135">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ad92b-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ad92b-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="ad92b-136">userEmailAddress</span></span>|<span data-ttu-id="ad92b-137">String</span><span class="sxs-lookup"><span data-stu-id="ad92b-137">String</span></span>|<span data-ttu-id="ad92b-138">ユーザーの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="ad92b-138">The user email address.</span></span> <span data-ttu-id="ad92b-139">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ad92b-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ad92b-140">userId</span><span class="sxs-lookup"><span data-stu-id="ad92b-140">userId</span></span>|<span data-ttu-id="ad92b-141">String</span><span class="sxs-lookup"><span data-stu-id="ad92b-141">String</span></span>|<span data-ttu-id="ad92b-142">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="ad92b-142">The user ID.</span></span> <span data-ttu-id="ad92b-143">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ad92b-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ad92b-144">userName</span><span class="sxs-lookup"><span data-stu-id="ad92b-144">userName</span></span>|<span data-ttu-id="ad92b-145">String</span><span class="sxs-lookup"><span data-stu-id="ad92b-145">String</span></span>|<span data-ttu-id="ad92b-146">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="ad92b-146">The user name.</span></span> <span data-ttu-id="ad92b-147">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ad92b-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ad92b-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ad92b-148">userPrincipalName</span></span>|<span data-ttu-id="ad92b-149">String</span><span class="sxs-lookup"><span data-stu-id="ad92b-149">String</span></span>|<span data-ttu-id="ad92b-150">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="ad92b-150">The user principal name.</span></span> <span data-ttu-id="ad92b-151">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ad92b-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ad92b-152">応答</span><span class="sxs-lookup"><span data-stu-id="ad92b-152">Response</span></span>
<span data-ttu-id="ad92b-153">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ad92b-153">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad92b-154">例</span><span class="sxs-lookup"><span data-stu-id="ad92b-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad92b-155">要求</span><span class="sxs-lookup"><span data-stu-id="ad92b-155">Request</span></span>
<span data-ttu-id="ad92b-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad92b-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
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

### <a name="response"></a><span data-ttu-id="ad92b-157">応答</span><span class="sxs-lookup"><span data-stu-id="ad92b-157">Response</span></span>
<span data-ttu-id="ad92b-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad92b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





