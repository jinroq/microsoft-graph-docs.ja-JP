---
title: ユーザーを更新する
description: ユーザー オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: dae6d6d16bfb1f849fa7a3a4e35e4c641718c70e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329429"
---
# <a name="update-user"></a><span data-ttu-id="e22fe-103">user の更新</span><span class="sxs-lookup"><span data-stu-id="e22fe-103">Update user</span></span>

> <span data-ttu-id="e22fe-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e22fe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e22fe-105">[user](../resources/intune-shared-user.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e22fe-105">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e22fe-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="e22fe-106">Prerequisites</span></span>
<span data-ttu-id="e22fe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e22fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e22fe-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e22fe-109">Permission type</span></span>|<span data-ttu-id="e22fe-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e22fe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e22fe-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e22fe-111">Delegated (work or school account)</span></span>| <span data-ttu-id="e22fe-112">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="e22fe-112">_varies by context_</span></span>|
| <span data-ttu-id="e22fe-113">&nbsp;&nbsp;デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="e22fe-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="e22fe-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e22fe-114">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="e22fe-115">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="e22fe-115">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="e22fe-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e22fe-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="e22fe-117">&nbsp;&nbsp;契約時</span><span class="sxs-lookup"><span data-stu-id="e22fe-117">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="e22fe-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e22fe-118">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e22fe-119">&nbsp;&nbsp;のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="e22fe-119">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="e22fe-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e22fe-120">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="e22fe-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e22fe-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e22fe-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e22fe-122">Not supported.</span></span>|
|<span data-ttu-id="e22fe-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e22fe-123">Application</span></span>|<span data-ttu-id="e22fe-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e22fe-124">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e22fe-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e22fe-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="e22fe-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e22fe-126">Request headers</span></span>
|<span data-ttu-id="e22fe-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e22fe-127">Header</span></span>|<span data-ttu-id="e22fe-128">値</span><span class="sxs-lookup"><span data-stu-id="e22fe-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e22fe-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e22fe-129">Authorization</span></span>|<span data-ttu-id="e22fe-130">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e22fe-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e22fe-131">Accept</span><span class="sxs-lookup"><span data-stu-id="e22fe-131">Accept</span></span>|<span data-ttu-id="e22fe-132">application/json</span><span class="sxs-lookup"><span data-stu-id="e22fe-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e22fe-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="e22fe-133">Request body</span></span>
<span data-ttu-id="e22fe-134">要求本文で、[user](../resources/intune-shared-user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e22fe-134">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="e22fe-135">次の表に、[user](../resources/intune-shared-user.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e22fe-135">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="e22fe-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e22fe-136">Property</span></span>|<span data-ttu-id="e22fe-137">種類</span><span class="sxs-lookup"><span data-stu-id="e22fe-137">Type</span></span>|<span data-ttu-id="e22fe-138">説明</span><span class="sxs-lookup"><span data-stu-id="e22fe-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e22fe-139">ID</span><span class="sxs-lookup"><span data-stu-id="e22fe-139">id</span></span>|<span data-ttu-id="e22fe-140">String</span><span class="sxs-lookup"><span data-stu-id="e22fe-140">String</span></span>|<span data-ttu-id="e22fe-141">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e22fe-141">Unique identifier of the user.</span></span>|
|<span data-ttu-id="e22fe-142">**契約時**</span><span class="sxs-lookup"><span data-stu-id="e22fe-142">**Onboarding**</span></span>|
|<span data-ttu-id="e22fe-143">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="e22fe-143">deviceEnrollmentLimit</span></span>|<span data-ttu-id="e22fe-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e22fe-144">Int32</span></span>|<span data-ttu-id="e22fe-145">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="e22fe-145">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="e22fe-146">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="e22fe-146">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="e22fe-147">応答</span><span class="sxs-lookup"><span data-stu-id="e22fe-147">Response</span></span>
<span data-ttu-id="e22fe-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [user](../resources/intune-shared-user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e22fe-148">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e22fe-149">例</span><span class="sxs-lookup"><span data-stu-id="e22fe-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="e22fe-150">要求</span><span class="sxs-lookup"><span data-stu-id="e22fe-150">Request</span></span>
<span data-ttu-id="e22fe-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e22fe-151">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="e22fe-152">応答</span><span class="sxs-lookup"><span data-stu-id="e22fe-152">Response</span></span>
<span data-ttu-id="e22fe-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e22fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



