---
title: MobileAppProvisioningConfigGroupAssignment を作成します。
description: 新しい mobileAppProvisioningConfigGroupAssignment オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 50b93e4858a7f986f5ebd25e8d2b09e204bae986
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417435"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="800bb-103">MobileAppProvisioningConfigGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="800bb-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="800bb-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="800bb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="800bb-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="800bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="800bb-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="800bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="800bb-107">新しい[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="800bb-107">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="800bb-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="800bb-108">Prerequisites</span></span>
<span data-ttu-id="800bb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="800bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="800bb-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="800bb-111">Permission type</span></span>|<span data-ttu-id="800bb-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="800bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="800bb-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="800bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="800bb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800bb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="800bb-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="800bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="800bb-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="800bb-116">Not supported.</span></span>|
|<span data-ttu-id="800bb-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="800bb-117">Application</span></span>|<span data-ttu-id="800bb-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="800bb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="800bb-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="800bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="800bb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="800bb-120">Request headers</span></span>
|<span data-ttu-id="800bb-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="800bb-121">Header</span></span>|<span data-ttu-id="800bb-122">値</span><span class="sxs-lookup"><span data-stu-id="800bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="800bb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="800bb-123">Authorization</span></span>|<span data-ttu-id="800bb-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="800bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="800bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="800bb-125">Accept</span></span>|<span data-ttu-id="800bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="800bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="800bb-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="800bb-127">Request body</span></span>
<span data-ttu-id="800bb-128">要求の本文に mobileAppProvisioningConfigGroupAssignment オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="800bb-128">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="800bb-129">次の表は、mobileAppProvisioningConfigGroupAssignment を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="800bb-129">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="800bb-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="800bb-130">Property</span></span>|<span data-ttu-id="800bb-131">型</span><span class="sxs-lookup"><span data-stu-id="800bb-131">Type</span></span>|<span data-ttu-id="800bb-132">説明</span><span class="sxs-lookup"><span data-stu-id="800bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="800bb-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="800bb-133">targetGroupId</span></span>|<span data-ttu-id="800bb-134">String</span><span class="sxs-lookup"><span data-stu-id="800bb-134">String</span></span>|<span data-ttu-id="800bb-135">構成のプロビジョニング、アプリケーションが対象である AAD グループの ID。</span><span class="sxs-lookup"><span data-stu-id="800bb-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="800bb-136">id</span><span class="sxs-lookup"><span data-stu-id="800bb-136">id</span></span>|<span data-ttu-id="800bb-137">String</span><span class="sxs-lookup"><span data-stu-id="800bb-137">String</span></span>|<span data-ttu-id="800bb-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="800bb-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="800bb-139">応答</span><span class="sxs-lookup"><span data-stu-id="800bb-139">Response</span></span>
<span data-ttu-id="800bb-140">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="800bb-140">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="800bb-141">例</span><span class="sxs-lookup"><span data-stu-id="800bb-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="800bb-142">要求</span><span class="sxs-lookup"><span data-stu-id="800bb-142">Request</span></span>
<span data-ttu-id="800bb-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="800bb-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="800bb-144">応答</span><span class="sxs-lookup"><span data-stu-id="800bb-144">Response</span></span>
<span data-ttu-id="800bb-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="800bb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




