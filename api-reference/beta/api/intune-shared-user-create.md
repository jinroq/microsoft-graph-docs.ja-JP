---
title: user の作成
description: 新しいユーザー オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9146f7292e003bb64c958e91d1305544b3980442
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821708"
---
# <a name="create-user"></a><span data-ttu-id="9257a-103">user の作成</span><span class="sxs-lookup"><span data-stu-id="9257a-103">Create user</span></span>

> <span data-ttu-id="9257a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9257a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9257a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9257a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9257a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9257a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9257a-107">新しい [user](../resources/intune-shared-user.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9257a-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9257a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9257a-108">Prerequisites</span></span>

<span data-ttu-id="9257a-109">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="9257a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9257a-110">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9257a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="9257a-111">必要な特定のアクセス許可は、コンテキストに依存します。</span><span class="sxs-lookup"><span data-stu-id="9257a-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="9257a-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9257a-112">Permission type</span></span>|<span data-ttu-id="9257a-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9257a-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9257a-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9257a-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9257a-115">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="9257a-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="9257a-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9257a-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="9257a-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="9257a-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="9257a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9257a-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="9257a-119">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="9257a-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="9257a-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9257a-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="9257a-121">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="9257a-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="9257a-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9257a-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9257a-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9257a-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9257a-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9257a-124">Not supported.</span></span>|
|<span data-ttu-id="9257a-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9257a-125">Application</span></span>|<span data-ttu-id="9257a-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9257a-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9257a-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9257a-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="9257a-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9257a-128">Request headers</span></span>

|<span data-ttu-id="9257a-129">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9257a-129">Header</span></span>|<span data-ttu-id="9257a-130">値</span><span class="sxs-lookup"><span data-stu-id="9257a-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9257a-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="9257a-131">Authorization</span></span>|<span data-ttu-id="9257a-132">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9257a-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9257a-133">Accept</span><span class="sxs-lookup"><span data-stu-id="9257a-133">Accept</span></span>|<span data-ttu-id="9257a-134">application/json</span><span class="sxs-lookup"><span data-stu-id="9257a-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9257a-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="9257a-135">Request body</span></span>

<span data-ttu-id="9257a-136">要求本文で、user オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9257a-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="9257a-137">次の表に、user の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9257a-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="9257a-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9257a-138">Property</span></span>|<span data-ttu-id="9257a-139">種類</span><span class="sxs-lookup"><span data-stu-id="9257a-139">Type</span></span>|<span data-ttu-id="9257a-140">説明</span><span class="sxs-lookup"><span data-stu-id="9257a-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9257a-141">ID</span><span class="sxs-lookup"><span data-stu-id="9257a-141">id</span></span>|<span data-ttu-id="9257a-142">String</span><span class="sxs-lookup"><span data-stu-id="9257a-142">String</span></span>|<span data-ttu-id="9257a-143">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="9257a-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="9257a-144">**採用**</span><span class="sxs-lookup"><span data-stu-id="9257a-144">**On-boarding**</span></span>||
|<span data-ttu-id="9257a-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="9257a-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="9257a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9257a-146">Int32</span></span>|<span data-ttu-id="9257a-147">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="9257a-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="9257a-148">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="9257a-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="9257a-149">要求本文のプロパティのサポートは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="9257a-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="9257a-150">応答</span><span class="sxs-lookup"><span data-stu-id="9257a-150">Response</span></span>

<span data-ttu-id="9257a-151">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [user](../resources/intune-shared-user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9257a-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9257a-152">例</span><span class="sxs-lookup"><span data-stu-id="9257a-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="9257a-153">要求</span><span class="sxs-lookup"><span data-stu-id="9257a-153">Request</span></span>

<span data-ttu-id="9257a-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9257a-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="9257a-155">応答</span><span class="sxs-lookup"><span data-stu-id="9257a-155">Response</span></span>

<span data-ttu-id="9257a-156">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9257a-156">Here is an example of the response.</span></span> <span data-ttu-id="9257a-157">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="9257a-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9257a-158">実際の呼び出しから返されるプロパティは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="9257a-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



