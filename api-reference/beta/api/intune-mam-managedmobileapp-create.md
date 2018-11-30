---
title: managedMobileApp の作成
description: 新しい managedMobileApp オブジェクトを作成します。
ms.openlocfilehash: cb62ebcf6649762ba86b68d94ce84893707954bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070531"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="095ab-103">managedMobileApp の作成</span><span class="sxs-lookup"><span data-stu-id="095ab-103">Create managedMobileApp</span></span>

> <span data-ttu-id="095ab-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="095ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="095ab-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="095ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="095ab-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="095ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="095ab-107">新しい [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="095ab-107">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="095ab-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="095ab-108">Prerequisites</span></span>
<span data-ttu-id="095ab-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="095ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="095ab-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="095ab-111">Permission type</span></span>|<span data-ttu-id="095ab-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="095ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="095ab-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="095ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="095ab-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="095ab-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="095ab-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="095ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="095ab-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="095ab-116">Not supported.</span></span>|
|<span data-ttu-id="095ab-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="095ab-117">Application</span></span>|<span data-ttu-id="095ab-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="095ab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="095ab-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="095ab-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="095ab-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="095ab-120">Request headers</span></span>
|<span data-ttu-id="095ab-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="095ab-121">Header</span></span>|<span data-ttu-id="095ab-122">値</span><span class="sxs-lookup"><span data-stu-id="095ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="095ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="095ab-123">Authorization</span></span>|<span data-ttu-id="095ab-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="095ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="095ab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="095ab-125">Accept</span></span>|<span data-ttu-id="095ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="095ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="095ab-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="095ab-127">Request body</span></span>
<span data-ttu-id="095ab-128">要求本文で、managedMobileApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="095ab-128">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="095ab-129">次の表に、managedMobileApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="095ab-129">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="095ab-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="095ab-130">Property</span></span>|<span data-ttu-id="095ab-131">型</span><span class="sxs-lookup"><span data-stu-id="095ab-131">Type</span></span>|<span data-ttu-id="095ab-132">説明</span><span class="sxs-lookup"><span data-stu-id="095ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="095ab-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="095ab-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="095ab-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="095ab-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="095ab-135">対象のオペレーティング システムの種類のアプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="095ab-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="095ab-136">id</span><span class="sxs-lookup"><span data-stu-id="095ab-136">id</span></span>|<span data-ttu-id="095ab-137">String</span><span class="sxs-lookup"><span data-stu-id="095ab-137">String</span></span>|<span data-ttu-id="095ab-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="095ab-138">Key of the entity.</span></span>|
|<span data-ttu-id="095ab-139">version</span><span class="sxs-lookup"><span data-stu-id="095ab-139">version</span></span>|<span data-ttu-id="095ab-140">String</span><span class="sxs-lookup"><span data-stu-id="095ab-140">String</span></span>|<span data-ttu-id="095ab-141">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="095ab-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="095ab-142">応答</span><span class="sxs-lookup"><span data-stu-id="095ab-142">Response</span></span>
<span data-ttu-id="095ab-143">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="095ab-143">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="095ab-144">例</span><span class="sxs-lookup"><span data-stu-id="095ab-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="095ab-145">要求</span><span class="sxs-lookup"><span data-stu-id="095ab-145">Request</span></span>
<span data-ttu-id="095ab-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="095ab-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="095ab-147">応答</span><span class="sxs-lookup"><span data-stu-id="095ab-147">Response</span></span>
<span data-ttu-id="095ab-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="095ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





