---
title: MobileAppProvisioningConfigGroupAssignment を作成します。
description: 新しい mobileAppProvisioningConfigGroupAssignment オブジェクトを作成します。
ms.openlocfilehash: 7ff1377079ea47d7bb809b9b71d1033a4681d19d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074316"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="a5b2c-103">MobileAppProvisioningConfigGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="a5b2c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5b2c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5b2c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5b2c-107">新しい[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-107">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a5b2c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a5b2c-108">Prerequisites</span></span>
<span data-ttu-id="a5b2c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5b2c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5b2c-111">Permission type</span></span>|<span data-ttu-id="a5b2c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5b2c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5b2c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5b2c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5b2c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5b2c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a5b2c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5b2c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5b2c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-116">Not supported.</span></span>|
|<span data-ttu-id="a5b2c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5b2c-117">Application</span></span>|<span data-ttu-id="a5b2c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5b2c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5b2c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a5b2c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5b2c-120">Request headers</span></span>
|<span data-ttu-id="a5b2c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5b2c-121">Header</span></span>|<span data-ttu-id="a5b2c-122">値</span><span class="sxs-lookup"><span data-stu-id="a5b2c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5b2c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5b2c-123">Authorization</span></span>|<span data-ttu-id="a5b2c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5b2c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5b2c-125">Accept</span></span>|<span data-ttu-id="a5b2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5b2c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5b2c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5b2c-127">Request body</span></span>
<span data-ttu-id="a5b2c-128">要求の本文に mobileAppProvisioningConfigGroupAssignment オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-128">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="a5b2c-129">次の表は、mobileAppProvisioningConfigGroupAssignment を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-129">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="a5b2c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5b2c-130">Property</span></span>|<span data-ttu-id="a5b2c-131">型</span><span class="sxs-lookup"><span data-stu-id="a5b2c-131">Type</span></span>|<span data-ttu-id="a5b2c-132">説明</span><span class="sxs-lookup"><span data-stu-id="a5b2c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5b2c-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="a5b2c-133">targetGroupId</span></span>|<span data-ttu-id="a5b2c-134">String</span><span class="sxs-lookup"><span data-stu-id="a5b2c-134">String</span></span>|<span data-ttu-id="a5b2c-135">構成のプロビジョニング、アプリケーションが対象である AAD グループの ID。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="a5b2c-136">id</span><span class="sxs-lookup"><span data-stu-id="a5b2c-136">id</span></span>|<span data-ttu-id="a5b2c-137">String</span><span class="sxs-lookup"><span data-stu-id="a5b2c-137">String</span></span>|<span data-ttu-id="a5b2c-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="a5b2c-139">応答</span><span class="sxs-lookup"><span data-stu-id="a5b2c-139">Response</span></span>
<span data-ttu-id="a5b2c-140">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-140">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5b2c-141">例</span><span class="sxs-lookup"><span data-stu-id="a5b2c-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5b2c-142">要求</span><span class="sxs-lookup"><span data-stu-id="a5b2c-142">Request</span></span>
<span data-ttu-id="a5b2c-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="a5b2c-144">応答</span><span class="sxs-lookup"><span data-stu-id="a5b2c-144">Response</span></span>
<span data-ttu-id="a5b2c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a5b2c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```





