---
title: deviceCategory の更新
description: deviceCategory オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 8676067ff4ce34358bcfd8400d28e1d73bd11f68
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321519"
---
# <a name="update-devicecategory"></a><span data-ttu-id="59015-103">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="59015-103">Update deviceCategory</span></span>

> <span data-ttu-id="59015-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="59015-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59015-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59015-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59015-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="59015-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59015-107">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="59015-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59015-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="59015-108">Prerequisites</span></span>

<span data-ttu-id="59015-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59015-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59015-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="59015-111">Permission type</span></span>|<span data-ttu-id="59015-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="59015-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59015-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="59015-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="59015-114">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="59015-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="59015-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59015-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="59015-116">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="59015-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="59015-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59015-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="59015-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="59015-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59015-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59015-119">Not supported.</span></span>|
|<span data-ttu-id="59015-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="59015-120">Application</span></span>|<span data-ttu-id="59015-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59015-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59015-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="59015-122">HTTP Request</span></span>

<span data-ttu-id="59015-123">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="59015-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="59015-124">**採用**</span><span class="sxs-lookup"><span data-stu-id="59015-124">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="59015-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59015-125">Request headers</span></span>

|<span data-ttu-id="59015-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59015-126">Header</span></span>|<span data-ttu-id="59015-127">値</span><span class="sxs-lookup"><span data-stu-id="59015-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59015-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="59015-128">Authorization</span></span>|<span data-ttu-id="59015-129">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="59015-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59015-130">Accept</span><span class="sxs-lookup"><span data-stu-id="59015-130">Accept</span></span>|<span data-ttu-id="59015-131">application/json</span><span class="sxs-lookup"><span data-stu-id="59015-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59015-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="59015-132">Request body</span></span>

<span data-ttu-id="59015-133">要求本文で、[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="59015-133">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="59015-134">次の表に、[deviceCategory](../resources/intune-shared-devicecategory.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="59015-134">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="59015-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59015-135">Property</span></span>|<span data-ttu-id="59015-136">種類</span><span class="sxs-lookup"><span data-stu-id="59015-136">Type</span></span>|<span data-ttu-id="59015-137">説明</span><span class="sxs-lookup"><span data-stu-id="59015-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59015-138">ID</span><span class="sxs-lookup"><span data-stu-id="59015-138">id</span></span>|<span data-ttu-id="59015-139">String</span><span class="sxs-lookup"><span data-stu-id="59015-139">String</span></span>|<span data-ttu-id="59015-140">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="59015-140">Unique identifier for the device category.</span></span> <span data-ttu-id="59015-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="59015-141">Read-only.</span></span>|
|<span data-ttu-id="59015-142">**契約時**</span><span class="sxs-lookup"><span data-stu-id="59015-142">**Onboarding**</span></span>|
|<span data-ttu-id="59015-143">説明</span><span class="sxs-lookup"><span data-stu-id="59015-143">description</span></span>|<span data-ttu-id="59015-144">String</span><span class="sxs-lookup"><span data-stu-id="59015-144">String</span></span>|<span data-ttu-id="59015-145">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="59015-145">Optional description for the device category.</span></span>|
|<span data-ttu-id="59015-146">displayName</span><span class="sxs-lookup"><span data-stu-id="59015-146">displayName</span></span>|<span data-ttu-id="59015-147">String</span><span class="sxs-lookup"><span data-stu-id="59015-147">String</span></span>|<span data-ttu-id="59015-148">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="59015-148">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="59015-149">応答</span><span class="sxs-lookup"><span data-stu-id="59015-149">Response</span></span>

<span data-ttu-id="59015-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="59015-150">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59015-151">例</span><span class="sxs-lookup"><span data-stu-id="59015-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="59015-152">要求</span><span class="sxs-lookup"><span data-stu-id="59015-152">Request</span></span>

<span data-ttu-id="59015-153">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59015-153">Here are examples of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="59015-154">応答</span><span class="sxs-lookup"><span data-stu-id="59015-154">Response</span></span>

<span data-ttu-id="59015-155">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="59015-155">Here is an example of the response.</span></span> <span data-ttu-id="59015-156">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="59015-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="59015-157">応答のプロパティは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="59015-157">Response properties will vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



