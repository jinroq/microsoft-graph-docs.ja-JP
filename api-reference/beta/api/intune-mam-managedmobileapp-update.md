---
title: managedMobileApp の更新
description: managedMobileApp オブジェクトのプロパティを更新します。
ms.openlocfilehash: c15e46562b43aa87f9dafe85be2b8dde93ff21f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067024"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="58d5a-103">managedMobileApp の更新</span><span class="sxs-lookup"><span data-stu-id="58d5a-103">Update managedMobileApp</span></span>

> <span data-ttu-id="58d5a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="58d5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58d5a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58d5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58d5a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="58d5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58d5a-107">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="58d5a-107">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58d5a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="58d5a-108">Prerequisites</span></span>
<span data-ttu-id="58d5a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58d5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58d5a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58d5a-111">Permission type</span></span>|<span data-ttu-id="58d5a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="58d5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58d5a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58d5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58d5a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58d5a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="58d5a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58d5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58d5a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58d5a-116">Not supported.</span></span>|
|<span data-ttu-id="58d5a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58d5a-117">Application</span></span>|<span data-ttu-id="58d5a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58d5a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58d5a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58d5a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="58d5a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58d5a-120">Request headers</span></span>
|<span data-ttu-id="58d5a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58d5a-121">Header</span></span>|<span data-ttu-id="58d5a-122">値</span><span class="sxs-lookup"><span data-stu-id="58d5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58d5a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58d5a-123">Authorization</span></span>|<span data-ttu-id="58d5a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="58d5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58d5a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58d5a-125">Accept</span></span>|<span data-ttu-id="58d5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58d5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58d5a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="58d5a-127">Request body</span></span>
<span data-ttu-id="58d5a-128">要求本文で、[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="58d5a-128">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="58d5a-129">次の表に、[managedMobileApp](../resources/intune-mam-managedmobileapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="58d5a-129">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="58d5a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58d5a-130">Property</span></span>|<span data-ttu-id="58d5a-131">型</span><span class="sxs-lookup"><span data-stu-id="58d5a-131">Type</span></span>|<span data-ttu-id="58d5a-132">説明</span><span class="sxs-lookup"><span data-stu-id="58d5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58d5a-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="58d5a-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="58d5a-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="58d5a-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="58d5a-135">対象のオペレーティング システムの種類のアプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="58d5a-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="58d5a-136">id</span><span class="sxs-lookup"><span data-stu-id="58d5a-136">id</span></span>|<span data-ttu-id="58d5a-137">String</span><span class="sxs-lookup"><span data-stu-id="58d5a-137">String</span></span>|<span data-ttu-id="58d5a-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="58d5a-138">Key of the entity.</span></span>|
|<span data-ttu-id="58d5a-139">version</span><span class="sxs-lookup"><span data-stu-id="58d5a-139">version</span></span>|<span data-ttu-id="58d5a-140">String</span><span class="sxs-lookup"><span data-stu-id="58d5a-140">String</span></span>|<span data-ttu-id="58d5a-141">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="58d5a-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="58d5a-142">応答</span><span class="sxs-lookup"><span data-stu-id="58d5a-142">Response</span></span>
<span data-ttu-id="58d5a-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="58d5a-143">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58d5a-144">例</span><span class="sxs-lookup"><span data-stu-id="58d5a-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="58d5a-145">要求</span><span class="sxs-lookup"><span data-stu-id="58d5a-145">Request</span></span>
<span data-ttu-id="58d5a-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="58d5a-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 126

{
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="58d5a-147">応答</span><span class="sxs-lookup"><span data-stu-id="58d5a-147">Response</span></span>
<span data-ttu-id="58d5a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="58d5a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





