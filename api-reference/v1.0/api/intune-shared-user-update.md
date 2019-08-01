---
title: ユーザーを更新する
description: ユーザー オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45307fcf1ff7f784a8fabcf3c6883b1a2faae258
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025758"
---
# <a name="update-user"></a><span data-ttu-id="134be-103">ユーザーを更新する</span><span class="sxs-lookup"><span data-stu-id="134be-103">Update user</span></span>

> <span data-ttu-id="134be-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="134be-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="134be-105">[user](../resources/intune-shared-user.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="134be-105">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="134be-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="134be-106">Prerequisites</span></span>
<span data-ttu-id="134be-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="134be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="134be-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="134be-109">Permission type</span></span>|<span data-ttu-id="134be-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="134be-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="134be-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="134be-111">Delegated (work or school account)</span></span>| <span data-ttu-id="134be-112">_コンテキストによって異なる_</span><span class="sxs-lookup"><span data-stu-id="134be-112">_varies by context_</span></span>|
| <span data-ttu-id="134be-113">&nbsp;&nbsp;デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="134be-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="134be-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="134be-114">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="134be-115">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="134be-115">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="134be-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="134be-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="134be-117">&nbsp;&nbsp;オンボード</span><span class="sxs-lookup"><span data-stu-id="134be-117">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="134be-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="134be-118">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="134be-119">&nbsp;&nbsp;トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="134be-119">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="134be-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="134be-120">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="134be-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="134be-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="134be-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="134be-122">Not supported.</span></span>|
|<span data-ttu-id="134be-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="134be-123">Application</span></span>|<span data-ttu-id="134be-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="134be-124">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="134be-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="134be-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="134be-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="134be-126">Request headers</span></span>
|<span data-ttu-id="134be-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="134be-127">Header</span></span>|<span data-ttu-id="134be-128">値</span><span class="sxs-lookup"><span data-stu-id="134be-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="134be-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="134be-129">Authorization</span></span>|<span data-ttu-id="134be-130">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="134be-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="134be-131">承諾</span><span class="sxs-lookup"><span data-stu-id="134be-131">Accept</span></span>|<span data-ttu-id="134be-132">application/json</span><span class="sxs-lookup"><span data-stu-id="134be-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="134be-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="134be-133">Request body</span></span>
<span data-ttu-id="134be-134">要求本文で、[user](../resources/intune-shared-user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="134be-134">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="134be-135">次の表に、[user](../resources/intune-shared-user.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="134be-135">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="134be-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="134be-136">Property</span></span>|<span data-ttu-id="134be-137">型</span><span class="sxs-lookup"><span data-stu-id="134be-137">Type</span></span>|<span data-ttu-id="134be-138">説明</span><span class="sxs-lookup"><span data-stu-id="134be-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="134be-139">id</span><span class="sxs-lookup"><span data-stu-id="134be-139">id</span></span>|<span data-ttu-id="134be-140">String</span><span class="sxs-lookup"><span data-stu-id="134be-140">String</span></span>|<span data-ttu-id="134be-141">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="134be-141">Unique identifier of the user.</span></span>|
|<span data-ttu-id="134be-142">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="134be-142">**Onboarding**</span></span>|
|<span data-ttu-id="134be-143">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="134be-143">deviceEnrollmentLimit</span></span>|<span data-ttu-id="134be-144">Int32</span><span class="sxs-lookup"><span data-stu-id="134be-144">Int32</span></span>|<span data-ttu-id="134be-145">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="134be-145">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="134be-146">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="134be-146">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="134be-147">応答</span><span class="sxs-lookup"><span data-stu-id="134be-147">Response</span></span>
<span data-ttu-id="134be-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [user](../resources/intune-shared-user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="134be-148">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="134be-149">例</span><span class="sxs-lookup"><span data-stu-id="134be-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="134be-150">要求</span><span class="sxs-lookup"><span data-stu-id="134be-150">Request</span></span>
<span data-ttu-id="134be-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="134be-151">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="134be-152">応答</span><span class="sxs-lookup"><span data-stu-id="134be-152">Response</span></span>
<span data-ttu-id="134be-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="134be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



