---
title: managedMobileApp の更新
description: managedMobileApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab9516fb0f44ceb959e39afc030fe2d826ab927c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548510"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="d180f-103">managedMobileApp の更新</span><span class="sxs-lookup"><span data-stu-id="d180f-103">Update managedMobileApp</span></span>

> <span data-ttu-id="d180f-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d180f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d180f-105">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d180f-105">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d180f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d180f-106">Prerequisites</span></span>
<span data-ttu-id="d180f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d180f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d180f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d180f-109">Permission type</span></span>|<span data-ttu-id="d180f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d180f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d180f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d180f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d180f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d180f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d180f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d180f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d180f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d180f-114">Not supported.</span></span>|
|<span data-ttu-id="d180f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d180f-115">Application</span></span>|<span data-ttu-id="d180f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d180f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d180f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d180f-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d180f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d180f-118">Request headers</span></span>
|<span data-ttu-id="d180f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d180f-119">Header</span></span>|<span data-ttu-id="d180f-120">値</span><span class="sxs-lookup"><span data-stu-id="d180f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d180f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d180f-121">Authorization</span></span>|<span data-ttu-id="d180f-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d180f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d180f-123">承諾</span><span class="sxs-lookup"><span data-stu-id="d180f-123">Accept</span></span>|<span data-ttu-id="d180f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d180f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d180f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d180f-125">Request body</span></span>
<span data-ttu-id="d180f-126">要求本文で、[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d180f-126">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="d180f-127">次の表に、[managedMobileApp](../resources/intune-mam-managedmobileapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d180f-127">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="d180f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d180f-128">Property</span></span>|<span data-ttu-id="d180f-129">型</span><span class="sxs-lookup"><span data-stu-id="d180f-129">Type</span></span>|<span data-ttu-id="d180f-130">説明</span><span class="sxs-lookup"><span data-stu-id="d180f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d180f-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d180f-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="d180f-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d180f-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d180f-133">対象のオペレーティング システムの種類のアプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="d180f-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="d180f-134">id</span><span class="sxs-lookup"><span data-stu-id="d180f-134">id</span></span>|<span data-ttu-id="d180f-135">String</span><span class="sxs-lookup"><span data-stu-id="d180f-135">String</span></span>|<span data-ttu-id="d180f-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d180f-136">Key of the entity.</span></span>|
|<span data-ttu-id="d180f-137">version</span><span class="sxs-lookup"><span data-stu-id="d180f-137">version</span></span>|<span data-ttu-id="d180f-138">String</span><span class="sxs-lookup"><span data-stu-id="d180f-138">String</span></span>|<span data-ttu-id="d180f-139">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d180f-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="d180f-140">応答</span><span class="sxs-lookup"><span data-stu-id="d180f-140">Response</span></span>
<span data-ttu-id="d180f-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d180f-141">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d180f-142">例</span><span class="sxs-lookup"><span data-stu-id="d180f-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="d180f-143">要求</span><span class="sxs-lookup"><span data-stu-id="d180f-143">Request</span></span>
<span data-ttu-id="d180f-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d180f-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
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

### <a name="response"></a><span data-ttu-id="d180f-145">応答</span><span class="sxs-lookup"><span data-stu-id="d180f-145">Response</span></span>
<span data-ttu-id="d180f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d180f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



