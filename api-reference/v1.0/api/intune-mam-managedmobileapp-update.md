---
title: managedMobileApp の更新
description: managedMobileApp オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 7dc10fa3d7272c2042712d385425504885020f1e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321099"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="6ff3a-103">managedMobileApp の更新</span><span class="sxs-lookup"><span data-stu-id="6ff3a-103">Update managedMobileApp</span></span>

> <span data-ttu-id="6ff3a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ff3a-105">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-105">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ff3a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6ff3a-106">Prerequisites</span></span>
<span data-ttu-id="6ff3a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ff3a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6ff3a-109">Permission type</span></span>|<span data-ttu-id="6ff3a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6ff3a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ff3a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6ff3a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6ff3a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ff3a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6ff3a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ff3a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ff3a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-114">Not supported.</span></span>|
|<span data-ttu-id="6ff3a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6ff3a-115">Application</span></span>|<span data-ttu-id="6ff3a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ff3a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6ff3a-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6ff3a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ff3a-118">Request headers</span></span>
|<span data-ttu-id="6ff3a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ff3a-119">Header</span></span>|<span data-ttu-id="6ff3a-120">値</span><span class="sxs-lookup"><span data-stu-id="6ff3a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ff3a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ff3a-121">Authorization</span></span>|<span data-ttu-id="6ff3a-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ff3a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6ff3a-123">Accept</span></span>|<span data-ttu-id="6ff3a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6ff3a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ff3a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6ff3a-125">Request body</span></span>
<span data-ttu-id="6ff3a-126">要求本文で、[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-126">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="6ff3a-127">次の表に、[managedMobileApp](../resources/intune-mam-managedmobileapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-127">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="6ff3a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ff3a-128">Property</span></span>|<span data-ttu-id="6ff3a-129">種類</span><span class="sxs-lookup"><span data-stu-id="6ff3a-129">Type</span></span>|<span data-ttu-id="6ff3a-130">説明</span><span class="sxs-lookup"><span data-stu-id="6ff3a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff3a-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6ff3a-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="6ff3a-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6ff3a-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="6ff3a-133">対象のオペレーティング システムの種類のアプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="6ff3a-134">id</span><span class="sxs-lookup"><span data-stu-id="6ff3a-134">id</span></span>|<span data-ttu-id="6ff3a-135">String</span><span class="sxs-lookup"><span data-stu-id="6ff3a-135">String</span></span>|<span data-ttu-id="6ff3a-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-136">Key of the entity.</span></span>|
|<span data-ttu-id="6ff3a-137">version</span><span class="sxs-lookup"><span data-stu-id="6ff3a-137">version</span></span>|<span data-ttu-id="6ff3a-138">String</span><span class="sxs-lookup"><span data-stu-id="6ff3a-138">String</span></span>|<span data-ttu-id="6ff3a-139">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="6ff3a-140">応答</span><span class="sxs-lookup"><span data-stu-id="6ff3a-140">Response</span></span>
<span data-ttu-id="6ff3a-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-141">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ff3a-142">例</span><span class="sxs-lookup"><span data-stu-id="6ff3a-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ff3a-143">要求</span><span class="sxs-lookup"><span data-stu-id="6ff3a-143">Request</span></span>
<span data-ttu-id="6ff3a-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6ff3a-145">応答</span><span class="sxs-lookup"><span data-stu-id="6ff3a-145">Response</span></span>
<span data-ttu-id="6ff3a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6ff3a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



