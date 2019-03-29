---
title: managedMobileApp の作成
description: 新しい managedMobileApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b001c8242ae207662feb8927ad8613054457620
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980125"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="7d29d-103">managedMobileApp の作成</span><span class="sxs-lookup"><span data-stu-id="7d29d-103">Create managedMobileApp</span></span>

> <span data-ttu-id="7d29d-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d29d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d29d-105">新しい [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7d29d-105">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d29d-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="7d29d-106">Prerequisites</span></span>
<span data-ttu-id="7d29d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d29d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d29d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d29d-109">Permission type</span></span>|<span data-ttu-id="7d29d-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d29d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d29d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d29d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d29d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d29d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d29d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d29d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d29d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d29d-114">Not supported.</span></span>|
|<span data-ttu-id="7d29d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d29d-115">Application</span></span>|<span data-ttu-id="7d29d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d29d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d29d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d29d-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="7d29d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d29d-118">Request headers</span></span>
|<span data-ttu-id="7d29d-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d29d-119">Header</span></span>|<span data-ttu-id="7d29d-120">値</span><span class="sxs-lookup"><span data-stu-id="7d29d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d29d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d29d-121">Authorization</span></span>|<span data-ttu-id="7d29d-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d29d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d29d-123">承諾</span><span class="sxs-lookup"><span data-stu-id="7d29d-123">Accept</span></span>|<span data-ttu-id="7d29d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7d29d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d29d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d29d-125">Request body</span></span>
<span data-ttu-id="7d29d-126">要求本文で、managedMobileApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d29d-126">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="7d29d-127">次の表に、managedMobileApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7d29d-127">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="7d29d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d29d-128">Property</span></span>|<span data-ttu-id="7d29d-129">型</span><span class="sxs-lookup"><span data-stu-id="7d29d-129">Type</span></span>|<span data-ttu-id="7d29d-130">説明</span><span class="sxs-lookup"><span data-stu-id="7d29d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d29d-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="7d29d-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="7d29d-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="7d29d-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="7d29d-133">対象のオペレーティング システムの種類のアプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="7d29d-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="7d29d-134">id</span><span class="sxs-lookup"><span data-stu-id="7d29d-134">id</span></span>|<span data-ttu-id="7d29d-135">String</span><span class="sxs-lookup"><span data-stu-id="7d29d-135">String</span></span>|<span data-ttu-id="7d29d-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7d29d-136">Key of the entity.</span></span>|
|<span data-ttu-id="7d29d-137">version</span><span class="sxs-lookup"><span data-stu-id="7d29d-137">version</span></span>|<span data-ttu-id="7d29d-138">String</span><span class="sxs-lookup"><span data-stu-id="7d29d-138">String</span></span>|<span data-ttu-id="7d29d-139">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="7d29d-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="7d29d-140">応答</span><span class="sxs-lookup"><span data-stu-id="7d29d-140">Response</span></span>
<span data-ttu-id="7d29d-141">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7d29d-141">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d29d-142">例</span><span class="sxs-lookup"><span data-stu-id="7d29d-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d29d-143">要求</span><span class="sxs-lookup"><span data-stu-id="7d29d-143">Request</span></span>
<span data-ttu-id="7d29d-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7d29d-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
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

### <a name="response"></a><span data-ttu-id="7d29d-145">応答</span><span class="sxs-lookup"><span data-stu-id="7d29d-145">Response</span></span>
<span data-ttu-id="7d29d-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7d29d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



