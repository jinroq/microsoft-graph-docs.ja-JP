---
title: deviceCategory の更新
description: deviceCategory オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90f5305e2fb52b5ecd184aad837f2c9d8f6334ef
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970101"
---
# <a name="update-devicecategory"></a><span data-ttu-id="5d47b-103">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="5d47b-103">Update deviceCategory</span></span>

> <span data-ttu-id="5d47b-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5d47b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5d47b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d47b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d47b-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5d47b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d47b-107">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5d47b-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d47b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5d47b-108">Prerequisites</span></span>

<span data-ttu-id="5d47b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d47b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d47b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5d47b-111">Permission type</span></span>|<span data-ttu-id="5d47b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5d47b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d47b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5d47b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5d47b-114">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="5d47b-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5d47b-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d47b-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="5d47b-116">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="5d47b-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5d47b-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d47b-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5d47b-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5d47b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d47b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d47b-119">Not supported.</span></span>|
|<span data-ttu-id="5d47b-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5d47b-120">Application</span></span>|<span data-ttu-id="5d47b-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d47b-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d47b-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5d47b-122">HTTP Request</span></span>

<span data-ttu-id="5d47b-123">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="5d47b-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="5d47b-124">**オンボード**</span><span class="sxs-lookup"><span data-stu-id="5d47b-124">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="5d47b-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d47b-125">Request headers</span></span>

|<span data-ttu-id="5d47b-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d47b-126">Header</span></span>|<span data-ttu-id="5d47b-127">値</span><span class="sxs-lookup"><span data-stu-id="5d47b-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d47b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d47b-128">Authorization</span></span>|<span data-ttu-id="5d47b-129">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5d47b-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d47b-130">承諾</span><span class="sxs-lookup"><span data-stu-id="5d47b-130">Accept</span></span>|<span data-ttu-id="5d47b-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5d47b-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d47b-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="5d47b-132">Request body</span></span>

<span data-ttu-id="5d47b-133">要求本文で、[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5d47b-133">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="5d47b-134">次の表に、[deviceCategory](../resources/intune-shared-devicecategory.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5d47b-134">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="5d47b-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d47b-135">Property</span></span>|<span data-ttu-id="5d47b-136">型</span><span class="sxs-lookup"><span data-stu-id="5d47b-136">Type</span></span>|<span data-ttu-id="5d47b-137">説明</span><span class="sxs-lookup"><span data-stu-id="5d47b-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d47b-138">id</span><span class="sxs-lookup"><span data-stu-id="5d47b-138">id</span></span>|<span data-ttu-id="5d47b-139">文字列</span><span class="sxs-lookup"><span data-stu-id="5d47b-139">String</span></span>|<span data-ttu-id="5d47b-140">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5d47b-140">Unique identifier for the device category.</span></span> <span data-ttu-id="5d47b-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5d47b-141">Read-only.</span></span>|
|<span data-ttu-id="5d47b-142">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="5d47b-142">**Onboarding**</span></span>|
|<span data-ttu-id="5d47b-143">description</span><span class="sxs-lookup"><span data-stu-id="5d47b-143">description</span></span>|<span data-ttu-id="5d47b-144">String</span><span class="sxs-lookup"><span data-stu-id="5d47b-144">String</span></span>|<span data-ttu-id="5d47b-145">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="5d47b-145">Optional description for the device category.</span></span>|
|<span data-ttu-id="5d47b-146">displayName</span><span class="sxs-lookup"><span data-stu-id="5d47b-146">displayName</span></span>|<span data-ttu-id="5d47b-147">String</span><span class="sxs-lookup"><span data-stu-id="5d47b-147">String</span></span>|<span data-ttu-id="5d47b-148">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="5d47b-148">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="5d47b-149">応答</span><span class="sxs-lookup"><span data-stu-id="5d47b-149">Response</span></span>

<span data-ttu-id="5d47b-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5d47b-150">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d47b-151">例</span><span class="sxs-lookup"><span data-stu-id="5d47b-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d47b-152">要求</span><span class="sxs-lookup"><span data-stu-id="5d47b-152">Request</span></span>

<span data-ttu-id="5d47b-153">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5d47b-153">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="5d47b-154">応答</span><span class="sxs-lookup"><span data-stu-id="5d47b-154">Response</span></span>

<span data-ttu-id="5d47b-155">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5d47b-155">Here is an example of the response.</span></span> <span data-ttu-id="5d47b-156">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="5d47b-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5d47b-157">応答プロパティは、状況に応じて異なります。</span><span class="sxs-lookup"><span data-stu-id="5d47b-157">Response properties will vary according to context.</span></span>

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



