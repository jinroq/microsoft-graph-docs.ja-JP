---
title: ユーザーを更新する
description: ユーザー オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f52e49c86e0e333fbf4f8c52b71c2850c73bc533
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861944"
---
# <a name="update-user"></a><span data-ttu-id="29d43-103">ユーザーを更新する</span><span class="sxs-lookup"><span data-stu-id="29d43-103">Update user</span></span>

> <span data-ttu-id="29d43-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中で、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="29d43-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29d43-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29d43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29d43-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="29d43-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29d43-107">[user](../resources/intune-shared-user.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="29d43-107">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29d43-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="29d43-108">Prerequisites</span></span>

<span data-ttu-id="29d43-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29d43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29d43-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29d43-111">Permission type</span></span>|<span data-ttu-id="29d43-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="29d43-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29d43-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29d43-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="29d43-114">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="29d43-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="29d43-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29d43-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="29d43-116">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="29d43-116">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="29d43-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29d43-117">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="29d43-118">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="29d43-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="29d43-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29d43-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="29d43-120">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="29d43-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="29d43-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29d43-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="29d43-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29d43-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29d43-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29d43-123">Not supported.</span></span>|
|<span data-ttu-id="29d43-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29d43-124">Application</span></span>|<span data-ttu-id="29d43-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29d43-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29d43-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29d43-126">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="29d43-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29d43-127">Request headers</span></span>

|<span data-ttu-id="29d43-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29d43-128">Header</span></span>|<span data-ttu-id="29d43-129">値</span><span class="sxs-lookup"><span data-stu-id="29d43-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29d43-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="29d43-130">Authorization</span></span>|<span data-ttu-id="29d43-131">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="29d43-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29d43-132">Accept</span><span class="sxs-lookup"><span data-stu-id="29d43-132">Accept</span></span>|<span data-ttu-id="29d43-133">application/json</span><span class="sxs-lookup"><span data-stu-id="29d43-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29d43-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="29d43-134">Request body</span></span>

<span data-ttu-id="29d43-135">要求本文で、[user](../resources/intune-shared-user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="29d43-135">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="29d43-136">次の表に、[user](../resources/intune-shared-user.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="29d43-136">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="29d43-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29d43-137">Property</span></span>|<span data-ttu-id="29d43-138">種類</span><span class="sxs-lookup"><span data-stu-id="29d43-138">Type</span></span>|<span data-ttu-id="29d43-139">説明</span><span class="sxs-lookup"><span data-stu-id="29d43-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29d43-140">ID</span><span class="sxs-lookup"><span data-stu-id="29d43-140">id</span></span>|<span data-ttu-id="29d43-141">String</span><span class="sxs-lookup"><span data-stu-id="29d43-141">String</span></span>|<span data-ttu-id="29d43-142">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="29d43-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="29d43-143">**契約時**</span><span class="sxs-lookup"><span data-stu-id="29d43-143">**Onboarding**</span></span>|
|<span data-ttu-id="29d43-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="29d43-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="29d43-145">Int32</span><span class="sxs-lookup"><span data-stu-id="29d43-145">Int32</span></span>|<span data-ttu-id="29d43-146">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="29d43-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="29d43-147">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="29d43-147">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="29d43-148">応答</span><span class="sxs-lookup"><span data-stu-id="29d43-148">Response</span></span>

<span data-ttu-id="29d43-149">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [user](../resources/intune-shared-user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="29d43-149">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29d43-150">例</span><span class="sxs-lookup"><span data-stu-id="29d43-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="29d43-151">要求</span><span class="sxs-lookup"><span data-stu-id="29d43-151">Request</span></span>

<span data-ttu-id="29d43-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="29d43-152">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="29d43-153">応答</span><span class="sxs-lookup"><span data-stu-id="29d43-153">Response</span></span>

<span data-ttu-id="29d43-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="29d43-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



