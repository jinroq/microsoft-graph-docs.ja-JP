---
title: deviceCategory の更新
description: deviceCategory オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0d34746c6047b5a61450361886483f3011523855
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943100"
---
# <a name="update-devicecategory"></a><span data-ttu-id="33e50-103">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="33e50-103">Update deviceCategory</span></span>

> <span data-ttu-id="33e50-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="33e50-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33e50-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33e50-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33e50-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="33e50-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33e50-107">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="33e50-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33e50-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="33e50-108">Prerequisites</span></span>

<span data-ttu-id="33e50-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33e50-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33e50-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33e50-111">Permission type</span></span>|<span data-ttu-id="33e50-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="33e50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33e50-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33e50-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="33e50-114">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="33e50-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="33e50-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33e50-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="33e50-116">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="33e50-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="33e50-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33e50-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="33e50-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33e50-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33e50-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33e50-119">Not supported.</span></span>|
|<span data-ttu-id="33e50-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33e50-120">Application</span></span>|<span data-ttu-id="33e50-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33e50-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33e50-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33e50-122">HTTP Request</span></span>

<span data-ttu-id="33e50-123">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="33e50-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="33e50-124">**採用**</span><span class="sxs-lookup"><span data-stu-id="33e50-124">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="33e50-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33e50-125">Request headers</span></span>

|<span data-ttu-id="33e50-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33e50-126">Header</span></span>|<span data-ttu-id="33e50-127">値</span><span class="sxs-lookup"><span data-stu-id="33e50-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33e50-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="33e50-128">Authorization</span></span>|<span data-ttu-id="33e50-129">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="33e50-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33e50-130">Accept</span><span class="sxs-lookup"><span data-stu-id="33e50-130">Accept</span></span>|<span data-ttu-id="33e50-131">application/json</span><span class="sxs-lookup"><span data-stu-id="33e50-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33e50-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="33e50-132">Request body</span></span>

<span data-ttu-id="33e50-133">要求本文で、[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="33e50-133">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="33e50-134">次の表に、[deviceCategory](../resources/intune-shared-devicecategory.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="33e50-134">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="33e50-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33e50-135">Property</span></span>|<span data-ttu-id="33e50-136">型</span><span class="sxs-lookup"><span data-stu-id="33e50-136">Type</span></span>|<span data-ttu-id="33e50-137">説明</span><span class="sxs-lookup"><span data-stu-id="33e50-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33e50-138">ID</span><span class="sxs-lookup"><span data-stu-id="33e50-138">id</span></span>|<span data-ttu-id="33e50-139">String</span><span class="sxs-lookup"><span data-stu-id="33e50-139">String</span></span>|<span data-ttu-id="33e50-140">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="33e50-140">Unique identifier for the device category.</span></span> <span data-ttu-id="33e50-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="33e50-141">Read-only.</span></span>|
|<span data-ttu-id="33e50-142">**契約時**</span><span class="sxs-lookup"><span data-stu-id="33e50-142">**Onboarding**</span></span>|
|<span data-ttu-id="33e50-143">説明</span><span class="sxs-lookup"><span data-stu-id="33e50-143">description</span></span>|<span data-ttu-id="33e50-144">String</span><span class="sxs-lookup"><span data-stu-id="33e50-144">String</span></span>|<span data-ttu-id="33e50-145">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="33e50-145">Optional description for the device category.</span></span>|
|<span data-ttu-id="33e50-146">displayName</span><span class="sxs-lookup"><span data-stu-id="33e50-146">displayName</span></span>|<span data-ttu-id="33e50-147">String</span><span class="sxs-lookup"><span data-stu-id="33e50-147">String</span></span>|<span data-ttu-id="33e50-148">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="33e50-148">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="33e50-149">応答</span><span class="sxs-lookup"><span data-stu-id="33e50-149">Response</span></span>

<span data-ttu-id="33e50-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="33e50-150">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33e50-151">例</span><span class="sxs-lookup"><span data-stu-id="33e50-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="33e50-152">要求</span><span class="sxs-lookup"><span data-stu-id="33e50-152">Request</span></span>

<span data-ttu-id="33e50-153">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="33e50-153">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="33e50-154">応答</span><span class="sxs-lookup"><span data-stu-id="33e50-154">Response</span></span>

<span data-ttu-id="33e50-155">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="33e50-155">Here is an example of the response.</span></span> <span data-ttu-id="33e50-156">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="33e50-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="33e50-157">応答のプロパティは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="33e50-157">Response properties will vary according to context.</span></span>

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



