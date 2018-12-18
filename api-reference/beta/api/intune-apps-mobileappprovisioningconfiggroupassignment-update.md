---
title: MobileAppProvisioningConfigGroupAssignment を更新します。
description: MobileAppProvisioningConfigGroupAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: c113c16234cb51146aa2e627d39405f740d6aab3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359144"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="7cff8-103">MobileAppProvisioningConfigGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="7cff8-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="7cff8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7cff8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7cff8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cff8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7cff8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7cff8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cff8-107">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7cff8-107">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7cff8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7cff8-108">Prerequisites</span></span>
<span data-ttu-id="7cff8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7cff8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cff8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7cff8-111">Permission type</span></span>|<span data-ttu-id="7cff8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7cff8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cff8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7cff8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7cff8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cff8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7cff8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7cff8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cff8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cff8-116">Not supported.</span></span>|
|<span data-ttu-id="7cff8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7cff8-117">Application</span></span>|<span data-ttu-id="7cff8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cff8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cff8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7cff8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7cff8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cff8-120">Request headers</span></span>
|<span data-ttu-id="7cff8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cff8-121">Header</span></span>|<span data-ttu-id="7cff8-122">値</span><span class="sxs-lookup"><span data-stu-id="7cff8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cff8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cff8-123">Authorization</span></span>|<span data-ttu-id="7cff8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7cff8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cff8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7cff8-125">Accept</span></span>|<span data-ttu-id="7cff8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7cff8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cff8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7cff8-127">Request body</span></span>
<span data-ttu-id="7cff8-128">要求の本文に[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="7cff8-128">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="7cff8-129">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="7cff8-129">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="7cff8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cff8-130">Property</span></span>|<span data-ttu-id="7cff8-131">種類</span><span class="sxs-lookup"><span data-stu-id="7cff8-131">Type</span></span>|<span data-ttu-id="7cff8-132">説明</span><span class="sxs-lookup"><span data-stu-id="7cff8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cff8-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="7cff8-133">targetGroupId</span></span>|<span data-ttu-id="7cff8-134">String</span><span class="sxs-lookup"><span data-stu-id="7cff8-134">String</span></span>|<span data-ttu-id="7cff8-135">構成のプロビジョニング、アプリケーションが対象である AAD グループの ID。</span><span class="sxs-lookup"><span data-stu-id="7cff8-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="7cff8-136">id</span><span class="sxs-lookup"><span data-stu-id="7cff8-136">id</span></span>|<span data-ttu-id="7cff8-137">String</span><span class="sxs-lookup"><span data-stu-id="7cff8-137">String</span></span>|<span data-ttu-id="7cff8-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7cff8-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="7cff8-139">応答</span><span class="sxs-lookup"><span data-stu-id="7cff8-139">Response</span></span>
<span data-ttu-id="7cff8-140">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7cff8-140">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cff8-141">例</span><span class="sxs-lookup"><span data-stu-id="7cff8-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="7cff8-142">要求</span><span class="sxs-lookup"><span data-stu-id="7cff8-142">Request</span></span>
<span data-ttu-id="7cff8-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7cff8-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 48

{
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="7cff8-144">応答</span><span class="sxs-lookup"><span data-stu-id="7cff8-144">Response</span></span>
<span data-ttu-id="7cff8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7cff8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```





