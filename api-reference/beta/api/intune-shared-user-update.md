---
title: ユーザーを更新する
description: ユーザー オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0009e563e34d40e8dae434761ed4203564ce9d9b
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571985"
---
# <a name="update-user"></a><span data-ttu-id="3fa0c-103">ユーザーを更新する</span><span class="sxs-lookup"><span data-stu-id="3fa0c-103">Update user</span></span>

> <span data-ttu-id="3fa0c-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3fa0c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fa0c-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fa0c-107">[user](../resources/intune-shared-user.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-107">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fa0c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3fa0c-108">Prerequisites</span></span>

<span data-ttu-id="3fa0c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3fa0c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3fa0c-111">Permission type</span></span>|<span data-ttu-id="3fa0c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3fa0c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fa0c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3fa0c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3fa0c-114">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="3fa0c-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="3fa0c-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa0c-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="3fa0c-116">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="3fa0c-116">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3fa0c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa0c-117">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="3fa0c-118">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="3fa0c-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="3fa0c-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa0c-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="3fa0c-120">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="3fa0c-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="3fa0c-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fa0c-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3fa0c-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3fa0c-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fa0c-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-123">Not supported.</span></span>|
|<span data-ttu-id="3fa0c-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3fa0c-124">Application</span></span>|<span data-ttu-id="3fa0c-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fa0c-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3fa0c-126">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="3fa0c-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3fa0c-127">Request headers</span></span>

|<span data-ttu-id="3fa0c-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3fa0c-128">Header</span></span>|<span data-ttu-id="3fa0c-129">値</span><span class="sxs-lookup"><span data-stu-id="3fa0c-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fa0c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fa0c-130">Authorization</span></span>|<span data-ttu-id="3fa0c-131">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fa0c-132">承諾</span><span class="sxs-lookup"><span data-stu-id="3fa0c-132">Accept</span></span>|<span data-ttu-id="3fa0c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="3fa0c-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fa0c-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="3fa0c-134">Request body</span></span>

<span data-ttu-id="3fa0c-135">要求本文で、[user](../resources/intune-shared-user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-135">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="3fa0c-136">次の表に、[user](../resources/intune-shared-user.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-136">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="3fa0c-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3fa0c-137">Property</span></span>|<span data-ttu-id="3fa0c-138">型</span><span class="sxs-lookup"><span data-stu-id="3fa0c-138">Type</span></span>|<span data-ttu-id="3fa0c-139">説明</span><span class="sxs-lookup"><span data-stu-id="3fa0c-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fa0c-140">id</span><span class="sxs-lookup"><span data-stu-id="3fa0c-140">id</span></span>|<span data-ttu-id="3fa0c-141">String</span><span class="sxs-lookup"><span data-stu-id="3fa0c-141">String</span></span>|<span data-ttu-id="3fa0c-142">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="3fa0c-143">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="3fa0c-143">**Onboarding**</span></span>|
|<span data-ttu-id="3fa0c-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="3fa0c-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="3fa0c-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3fa0c-145">Int32</span></span>|<span data-ttu-id="3fa0c-146">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="3fa0c-147">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-147">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="3fa0c-148">応答</span><span class="sxs-lookup"><span data-stu-id="3fa0c-148">Response</span></span>

<span data-ttu-id="3fa0c-149">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [user](../resources/intune-shared-user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-149">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fa0c-150">例</span><span class="sxs-lookup"><span data-stu-id="3fa0c-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fa0c-151">要求</span><span class="sxs-lookup"><span data-stu-id="3fa0c-151">Request</span></span>

<span data-ttu-id="3fa0c-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-152">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="3fa0c-153">応答</span><span class="sxs-lookup"><span data-stu-id="3fa0c-153">Response</span></span>

<span data-ttu-id="3fa0c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3fa0c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



