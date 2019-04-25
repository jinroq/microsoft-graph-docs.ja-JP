---
title: deviceCategory の更新
description: deviceCategory オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 831232fc656ad4aa0968e40aca5ae54b1e13ceef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576966"
---
# <a name="update-devicecategory"></a><span data-ttu-id="6b20f-103">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="6b20f-103">Update deviceCategory</span></span>

> <span data-ttu-id="6b20f-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b20f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b20f-105">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6b20f-105">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b20f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6b20f-106">Prerequisites</span></span>
<span data-ttu-id="6b20f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b20f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b20f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6b20f-109">Permission type</span></span>|<span data-ttu-id="6b20f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6b20f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b20f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6b20f-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6b20f-112">&nbsp;&nbsp; **オンボード**と</span><span class="sxs-lookup"><span data-stu-id="6b20f-112">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="6b20f-113">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="6b20f-113">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="6b20f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b20f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6b20f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b20f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b20f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b20f-116">Not supported.</span></span>|
|<span data-ttu-id="6b20f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6b20f-117">Application</span></span>|<span data-ttu-id="6b20f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b20f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b20f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6b20f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="6b20f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b20f-120">Request headers</span></span>
|<span data-ttu-id="6b20f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b20f-121">Header</span></span>|<span data-ttu-id="6b20f-122">値</span><span class="sxs-lookup"><span data-stu-id="6b20f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b20f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b20f-123">Authorization</span></span>|<span data-ttu-id="6b20f-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b20f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b20f-125">承諾</span><span class="sxs-lookup"><span data-stu-id="6b20f-125">Accept</span></span>|<span data-ttu-id="6b20f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b20f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b20f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6b20f-127">Request body</span></span>
<span data-ttu-id="6b20f-128">要求本文で、[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b20f-128">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="6b20f-129">次の表に、[deviceCategory](../resources/intune-shared-devicecategory.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6b20f-129">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="6b20f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b20f-130">Property</span></span>|<span data-ttu-id="6b20f-131">型</span><span class="sxs-lookup"><span data-stu-id="6b20f-131">Type</span></span>|<span data-ttu-id="6b20f-132">説明</span><span class="sxs-lookup"><span data-stu-id="6b20f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b20f-133">id</span><span class="sxs-lookup"><span data-stu-id="6b20f-133">id</span></span>|<span data-ttu-id="6b20f-134">文字列</span><span class="sxs-lookup"><span data-stu-id="6b20f-134">String</span></span>|<span data-ttu-id="6b20f-135">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6b20f-135">Unique identifier for the device category.</span></span> <span data-ttu-id="6b20f-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6b20f-136">Read-only.</span></span>|
|<span data-ttu-id="6b20f-137">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="6b20f-137">**Onboarding**</span></span>|
|<span data-ttu-id="6b20f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="6b20f-138">displayName</span></span>|<span data-ttu-id="6b20f-139">String</span><span class="sxs-lookup"><span data-stu-id="6b20f-139">String</span></span>|<span data-ttu-id="6b20f-140">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="6b20f-140">Display name for the device category.</span></span>|
|<span data-ttu-id="6b20f-141">説明</span><span class="sxs-lookup"><span data-stu-id="6b20f-141">description</span></span>|<span data-ttu-id="6b20f-142">String</span><span class="sxs-lookup"><span data-stu-id="6b20f-142">String</span></span>|<span data-ttu-id="6b20f-143">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="6b20f-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="6b20f-144">応答</span><span class="sxs-lookup"><span data-stu-id="6b20f-144">Response</span></span>
<span data-ttu-id="6b20f-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6b20f-145">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b20f-146">例</span><span class="sxs-lookup"><span data-stu-id="6b20f-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b20f-147">要求</span><span class="sxs-lookup"><span data-stu-id="6b20f-147">Request</span></span>
<span data-ttu-id="6b20f-148">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6b20f-148">Here are examples of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="6b20f-149">応答</span><span class="sxs-lookup"><span data-stu-id="6b20f-149">Response</span></span>
<span data-ttu-id="6b20f-150">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6b20f-150">Here is an example of the response.</span></span> <span data-ttu-id="6b20f-151">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6b20f-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6b20f-152">応答プロパティは、状況に応じて異なります。</span><span class="sxs-lookup"><span data-stu-id="6b20f-152">Response properties will vary according to context.</span></span>
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



