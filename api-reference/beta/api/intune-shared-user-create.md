---
title: user の作成
description: 新しいユーザー オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f46fbbc365e52ae9e46db9f6c05c3c8e8eeddc92
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572258"
---
# <a name="create-user"></a><span data-ttu-id="da7fd-103">ユーザーを作成する</span><span class="sxs-lookup"><span data-stu-id="da7fd-103">Create user</span></span>

> <span data-ttu-id="da7fd-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="da7fd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da7fd-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da7fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da7fd-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da7fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da7fd-107">新しい [user](../resources/intune-shared-user.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="da7fd-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da7fd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="da7fd-108">Prerequisites</span></span>

<span data-ttu-id="da7fd-109">この API を呼び出すには、次のいずれかのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="da7fd-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="da7fd-110">アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da7fd-110">To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>  <span data-ttu-id="da7fd-111">必要な特定のアクセス許可は、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="da7fd-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="da7fd-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da7fd-112">Permission type</span></span>|<span data-ttu-id="da7fd-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="da7fd-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da7fd-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da7fd-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="da7fd-115">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="da7fd-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="da7fd-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da7fd-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="da7fd-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="da7fd-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="da7fd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da7fd-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="da7fd-119">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="da7fd-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="da7fd-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da7fd-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="da7fd-121">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="da7fd-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="da7fd-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da7fd-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="da7fd-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da7fd-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da7fd-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da7fd-124">Not supported.</span></span>|
|<span data-ttu-id="da7fd-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da7fd-125">Application</span></span>|<span data-ttu-id="da7fd-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da7fd-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da7fd-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da7fd-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="da7fd-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da7fd-128">Request headers</span></span>

|<span data-ttu-id="da7fd-129">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da7fd-129">Header</span></span>|<span data-ttu-id="da7fd-130">値</span><span class="sxs-lookup"><span data-stu-id="da7fd-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da7fd-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="da7fd-131">Authorization</span></span>|<span data-ttu-id="da7fd-132">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="da7fd-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da7fd-133">承諾</span><span class="sxs-lookup"><span data-stu-id="da7fd-133">Accept</span></span>|<span data-ttu-id="da7fd-134">application/json</span><span class="sxs-lookup"><span data-stu-id="da7fd-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da7fd-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="da7fd-135">Request body</span></span>

<span data-ttu-id="da7fd-136">要求本文で、user オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="da7fd-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="da7fd-137">次の表に、user の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="da7fd-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="da7fd-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da7fd-138">Property</span></span>|<span data-ttu-id="da7fd-139">型</span><span class="sxs-lookup"><span data-stu-id="da7fd-139">Type</span></span>|<span data-ttu-id="da7fd-140">説明</span><span class="sxs-lookup"><span data-stu-id="da7fd-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da7fd-141">id</span><span class="sxs-lookup"><span data-stu-id="da7fd-141">id</span></span>|<span data-ttu-id="da7fd-142">String</span><span class="sxs-lookup"><span data-stu-id="da7fd-142">String</span></span>|<span data-ttu-id="da7fd-143">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="da7fd-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="da7fd-144">**オンボード**</span><span class="sxs-lookup"><span data-stu-id="da7fd-144">**On-boarding**</span></span>||
|<span data-ttu-id="da7fd-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="da7fd-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="da7fd-146">Int32</span><span class="sxs-lookup"><span data-stu-id="da7fd-146">Int32</span></span>|<span data-ttu-id="da7fd-147">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="da7fd-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="da7fd-148">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="da7fd-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="da7fd-149">要求本文のプロパティのサポートは、コンテキストに応じて異なります。</span><span class="sxs-lookup"><span data-stu-id="da7fd-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="da7fd-150">応答</span><span class="sxs-lookup"><span data-stu-id="da7fd-150">Response</span></span>

<span data-ttu-id="da7fd-151">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [user](../resources/intune-shared-user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="da7fd-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da7fd-152">例</span><span class="sxs-lookup"><span data-stu-id="da7fd-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="da7fd-153">要求</span><span class="sxs-lookup"><span data-stu-id="da7fd-153">Request</span></span>

<span data-ttu-id="da7fd-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="da7fd-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="da7fd-155">応答</span><span class="sxs-lookup"><span data-stu-id="da7fd-155">Response</span></span>

<span data-ttu-id="da7fd-156">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="da7fd-156">Here is an example of the response.</span></span> <span data-ttu-id="da7fd-157">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="da7fd-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="da7fd-158">実際の呼び出しから返されるプロパティは、コンテキストに応じて異なります。</span><span class="sxs-lookup"><span data-stu-id="da7fd-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



