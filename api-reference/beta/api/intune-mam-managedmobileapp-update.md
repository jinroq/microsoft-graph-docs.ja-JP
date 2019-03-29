---
title: managedMobileApp の更新
description: managedMobileApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 378c28bfee54090fd0802ff4c5ae61b262adf41f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972327"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="22f8c-103">managedMobileApp の更新</span><span class="sxs-lookup"><span data-stu-id="22f8c-103">Update managedMobileApp</span></span>

> <span data-ttu-id="22f8c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22f8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22f8c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22f8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22f8c-106">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="22f8c-106">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22f8c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="22f8c-107">Prerequisites</span></span>
<span data-ttu-id="22f8c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22f8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22f8c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22f8c-110">Permission type</span></span>|<span data-ttu-id="22f8c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="22f8c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22f8c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22f8c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22f8c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22f8c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22f8c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22f8c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22f8c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22f8c-115">Not supported.</span></span>|
|<span data-ttu-id="22f8c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22f8c-116">Application</span></span>|<span data-ttu-id="22f8c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22f8c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22f8c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22f8c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="22f8c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22f8c-119">Request headers</span></span>
|<span data-ttu-id="22f8c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22f8c-120">Header</span></span>|<span data-ttu-id="22f8c-121">値</span><span class="sxs-lookup"><span data-stu-id="22f8c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22f8c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22f8c-122">Authorization</span></span>|<span data-ttu-id="22f8c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="22f8c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22f8c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="22f8c-124">Accept</span></span>|<span data-ttu-id="22f8c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22f8c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22f8c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="22f8c-126">Request body</span></span>
<span data-ttu-id="22f8c-127">要求本文で、[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="22f8c-127">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="22f8c-128">次の表に、[managedMobileApp](../resources/intune-mam-managedmobileapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="22f8c-128">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="22f8c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22f8c-129">Property</span></span>|<span data-ttu-id="22f8c-130">型</span><span class="sxs-lookup"><span data-stu-id="22f8c-130">Type</span></span>|<span data-ttu-id="22f8c-131">説明</span><span class="sxs-lookup"><span data-stu-id="22f8c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22f8c-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="22f8c-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="22f8c-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="22f8c-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="22f8c-134">対象のオペレーティング システムの種類のアプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="22f8c-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="22f8c-135">id</span><span class="sxs-lookup"><span data-stu-id="22f8c-135">id</span></span>|<span data-ttu-id="22f8c-136">String</span><span class="sxs-lookup"><span data-stu-id="22f8c-136">String</span></span>|<span data-ttu-id="22f8c-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="22f8c-137">Key of the entity.</span></span>|
|<span data-ttu-id="22f8c-138">version</span><span class="sxs-lookup"><span data-stu-id="22f8c-138">version</span></span>|<span data-ttu-id="22f8c-139">String</span><span class="sxs-lookup"><span data-stu-id="22f8c-139">String</span></span>|<span data-ttu-id="22f8c-140">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="22f8c-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="22f8c-141">応答</span><span class="sxs-lookup"><span data-stu-id="22f8c-141">Response</span></span>
<span data-ttu-id="22f8c-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="22f8c-142">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22f8c-143">例</span><span class="sxs-lookup"><span data-stu-id="22f8c-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="22f8c-144">要求</span><span class="sxs-lookup"><span data-stu-id="22f8c-144">Request</span></span>
<span data-ttu-id="22f8c-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22f8c-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="22f8c-146">応答</span><span class="sxs-lookup"><span data-stu-id="22f8c-146">Response</span></span>
<span data-ttu-id="22f8c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22f8c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```




