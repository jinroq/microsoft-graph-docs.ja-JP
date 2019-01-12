---
title: user の作成
description: 新しいユーザー オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1b1789cbf0743384780147ce8c50f5472f9f2d64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981505"
---
# <a name="create-user"></a><span data-ttu-id="38947-103">user の作成</span><span class="sxs-lookup"><span data-stu-id="38947-103">Create user</span></span>

> <span data-ttu-id="38947-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="38947-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38947-105">新しい [user](../resources/intune-shared-user.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="38947-105">Create a new [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38947-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="38947-106">Prerequisites</span></span>
<span data-ttu-id="38947-107">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="38947-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="38947-108">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38947-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="38947-109">必要な特定のアクセス許可は、コンテキストに依存します。</span><span class="sxs-lookup"><span data-stu-id="38947-109">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="38947-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="38947-110">Permission type</span></span>|<span data-ttu-id="38947-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="38947-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38947-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="38947-112">Delegated (work or school account)</span></span>| <span data-ttu-id="38947-113">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="38947-113">_varies by context_</span></span> |
| <span data-ttu-id="38947-114">&nbsp;&nbsp;デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="38947-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="38947-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38947-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="38947-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="38947-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="38947-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38947-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="38947-118">&nbsp;&nbsp;契約時</span><span class="sxs-lookup"><span data-stu-id="38947-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="38947-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38947-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="38947-120">&nbsp;&nbsp;のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="38947-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="38947-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38947-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="38947-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="38947-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38947-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38947-123">Not supported.</span></span>|
|<span data-ttu-id="38947-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="38947-124">Application</span></span>|<span data-ttu-id="38947-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38947-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38947-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="38947-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="38947-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38947-127">Request headers</span></span>
|<span data-ttu-id="38947-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38947-128">Header</span></span>|<span data-ttu-id="38947-129">値</span><span class="sxs-lookup"><span data-stu-id="38947-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38947-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="38947-130">Authorization</span></span>|<span data-ttu-id="38947-131">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="38947-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38947-132">Accept</span><span class="sxs-lookup"><span data-stu-id="38947-132">Accept</span></span>|<span data-ttu-id="38947-133">application/json</span><span class="sxs-lookup"><span data-stu-id="38947-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38947-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="38947-134">Request body</span></span>
<span data-ttu-id="38947-135">要求本文で、user オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="38947-135">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="38947-136">次の表に、user の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="38947-136">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="38947-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38947-137">Property</span></span>|<span data-ttu-id="38947-138">型</span><span class="sxs-lookup"><span data-stu-id="38947-138">Type</span></span>|<span data-ttu-id="38947-139">説明</span><span class="sxs-lookup"><span data-stu-id="38947-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38947-140">ID</span><span class="sxs-lookup"><span data-stu-id="38947-140">id</span></span>|<span data-ttu-id="38947-141">String</span><span class="sxs-lookup"><span data-stu-id="38947-141">String</span></span>|<span data-ttu-id="38947-142">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="38947-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="38947-143">**契約時**</span><span class="sxs-lookup"><span data-stu-id="38947-143">**Onboarding**</span></span>|
|<span data-ttu-id="38947-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="38947-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="38947-145">Int32</span><span class="sxs-lookup"><span data-stu-id="38947-145">Int32</span></span>|<span data-ttu-id="38947-146">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="38947-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="38947-147">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="38947-147">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="38947-148">要求本文のプロパティのサポートは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="38947-148">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="38947-149">応答</span><span class="sxs-lookup"><span data-stu-id="38947-149">Response</span></span>
<span data-ttu-id="38947-150">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [user](../resources/intune-shared-user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="38947-150">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38947-151">例</span><span class="sxs-lookup"><span data-stu-id="38947-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="38947-152">要求</span><span class="sxs-lookup"><span data-stu-id="38947-152">Request</span></span>
<span data-ttu-id="38947-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="38947-153">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="38947-154">応答</span><span class="sxs-lookup"><span data-stu-id="38947-154">Response</span></span>
<span data-ttu-id="38947-155">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="38947-155">Here is an example of the response.</span></span> <span data-ttu-id="38947-156">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="38947-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="38947-157">実際の呼び出しから返されるプロパティは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="38947-157">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



