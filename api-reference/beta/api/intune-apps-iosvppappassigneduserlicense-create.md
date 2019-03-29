---
title: iosVppAppAssignedUserLicense を作成する
description: 新しい iosVppAppAssignedUserLicense オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e905316197453dfde89f8e074a8105b88d28e1c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970451"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="8601b-103">iosVppAppAssignedUserLicense を作成する</span><span class="sxs-lookup"><span data-stu-id="8601b-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="8601b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8601b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8601b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8601b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8601b-106">新しい[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8601b-106">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8601b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8601b-107">Prerequisites</span></span>
<span data-ttu-id="8601b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8601b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8601b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8601b-110">Permission type</span></span>|<span data-ttu-id="8601b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8601b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8601b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8601b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8601b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8601b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8601b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8601b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8601b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8601b-115">Not supported.</span></span>|
|<span data-ttu-id="8601b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8601b-116">Application</span></span>|<span data-ttu-id="8601b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8601b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8601b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8601b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="8601b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8601b-119">Request headers</span></span>
|<span data-ttu-id="8601b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8601b-120">Header</span></span>|<span data-ttu-id="8601b-121">値</span><span class="sxs-lookup"><span data-stu-id="8601b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8601b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8601b-122">Authorization</span></span>|<span data-ttu-id="8601b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8601b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8601b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8601b-124">Accept</span></span>|<span data-ttu-id="8601b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8601b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8601b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8601b-126">Request body</span></span>
<span data-ttu-id="8601b-127">要求本文で、iosVppAppAssignedUserLicense オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8601b-127">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="8601b-128">次の表に、iosVppAppAssignedUserLicense の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8601b-128">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="8601b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8601b-129">Property</span></span>|<span data-ttu-id="8601b-130">型</span><span class="sxs-lookup"><span data-stu-id="8601b-130">Type</span></span>|<span data-ttu-id="8601b-131">説明</span><span class="sxs-lookup"><span data-stu-id="8601b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8601b-132">id</span><span class="sxs-lookup"><span data-stu-id="8601b-132">id</span></span>|<span data-ttu-id="8601b-133">String</span><span class="sxs-lookup"><span data-stu-id="8601b-133">String</span></span>|<span data-ttu-id="8601b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8601b-134">Key of the entity.</span></span> <span data-ttu-id="8601b-135">[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8601b-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8601b-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8601b-136">userEmailAddress</span></span>|<span data-ttu-id="8601b-137">String</span><span class="sxs-lookup"><span data-stu-id="8601b-137">String</span></span>|<span data-ttu-id="8601b-138">ユーザーの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="8601b-138">The user email address.</span></span> <span data-ttu-id="8601b-139">[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8601b-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8601b-140">userId</span><span class="sxs-lookup"><span data-stu-id="8601b-140">userId</span></span>|<span data-ttu-id="8601b-141">String</span><span class="sxs-lookup"><span data-stu-id="8601b-141">String</span></span>|<span data-ttu-id="8601b-142">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="8601b-142">The user ID.</span></span> <span data-ttu-id="8601b-143">[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8601b-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8601b-144">userName</span><span class="sxs-lookup"><span data-stu-id="8601b-144">userName</span></span>|<span data-ttu-id="8601b-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8601b-145">String</span></span>|<span data-ttu-id="8601b-146">ユーザー名。</span><span class="sxs-lookup"><span data-stu-id="8601b-146">The user name.</span></span> <span data-ttu-id="8601b-147">[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8601b-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8601b-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8601b-148">userPrincipalName</span></span>|<span data-ttu-id="8601b-149">String</span><span class="sxs-lookup"><span data-stu-id="8601b-149">String</span></span>|<span data-ttu-id="8601b-150">ユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="8601b-150">The user principal name.</span></span> <span data-ttu-id="8601b-151">[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8601b-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8601b-152">応答</span><span class="sxs-lookup"><span data-stu-id="8601b-152">Response</span></span>
<span data-ttu-id="8601b-153">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8601b-153">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8601b-154">例</span><span class="sxs-lookup"><span data-stu-id="8601b-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="8601b-155">要求</span><span class="sxs-lookup"><span data-stu-id="8601b-155">Request</span></span>
<span data-ttu-id="8601b-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8601b-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8601b-157">応答</span><span class="sxs-lookup"><span data-stu-id="8601b-157">Response</span></span>
<span data-ttu-id="8601b-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8601b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




