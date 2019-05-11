---
title: managedMobileApp の作成
description: 新しい managedMobileApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f865b4921157e4591d216e6f55585688939fb61b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33903386"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="d3f40-103">managedMobileApp の作成</span><span class="sxs-lookup"><span data-stu-id="d3f40-103">Create managedMobileApp</span></span>

> <span data-ttu-id="d3f40-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3f40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3f40-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3f40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3f40-106">新しい [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d3f40-106">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3f40-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d3f40-107">Prerequisites</span></span>
<span data-ttu-id="d3f40-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3f40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3f40-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d3f40-110">Permission type</span></span>|<span data-ttu-id="d3f40-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d3f40-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3f40-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d3f40-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d3f40-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3f40-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d3f40-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d3f40-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3f40-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3f40-115">Not supported.</span></span>|
|<span data-ttu-id="d3f40-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d3f40-116">Application</span></span>|<span data-ttu-id="d3f40-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3f40-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3f40-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d3f40-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
POST /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="d3f40-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3f40-119">Request headers</span></span>
|<span data-ttu-id="d3f40-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3f40-120">Header</span></span>|<span data-ttu-id="d3f40-121">値</span><span class="sxs-lookup"><span data-stu-id="d3f40-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3f40-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3f40-122">Authorization</span></span>|<span data-ttu-id="d3f40-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3f40-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3f40-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d3f40-124">Accept</span></span>|<span data-ttu-id="d3f40-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3f40-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3f40-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d3f40-126">Request body</span></span>
<span data-ttu-id="d3f40-127">要求本文で、managedMobileApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d3f40-127">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="d3f40-128">次の表に、managedMobileApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d3f40-128">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="d3f40-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3f40-129">Property</span></span>|<span data-ttu-id="d3f40-130">型</span><span class="sxs-lookup"><span data-stu-id="d3f40-130">Type</span></span>|<span data-ttu-id="d3f40-131">説明</span><span class="sxs-lookup"><span data-stu-id="d3f40-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3f40-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d3f40-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="d3f40-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d3f40-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d3f40-134">対象のオペレーティング システムの種類のアプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="d3f40-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="d3f40-135">id</span><span class="sxs-lookup"><span data-stu-id="d3f40-135">id</span></span>|<span data-ttu-id="d3f40-136">String</span><span class="sxs-lookup"><span data-stu-id="d3f40-136">String</span></span>|<span data-ttu-id="d3f40-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d3f40-137">Key of the entity.</span></span>|
|<span data-ttu-id="d3f40-138">version</span><span class="sxs-lookup"><span data-stu-id="d3f40-138">version</span></span>|<span data-ttu-id="d3f40-139">String</span><span class="sxs-lookup"><span data-stu-id="d3f40-139">String</span></span>|<span data-ttu-id="d3f40-140">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d3f40-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="d3f40-141">応答</span><span class="sxs-lookup"><span data-stu-id="d3f40-141">Response</span></span>
<span data-ttu-id="d3f40-142">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d3f40-142">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3f40-143">例</span><span class="sxs-lookup"><span data-stu-id="d3f40-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3f40-144">要求</span><span class="sxs-lookup"><span data-stu-id="d3f40-144">Request</span></span>
<span data-ttu-id="d3f40-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d3f40-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
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

### <a name="response"></a><span data-ttu-id="d3f40-146">応答</span><span class="sxs-lookup"><span data-stu-id="d3f40-146">Response</span></span>
<span data-ttu-id="d3f40-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d3f40-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




