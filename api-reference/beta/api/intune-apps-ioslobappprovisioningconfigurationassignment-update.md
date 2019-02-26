---
title: ioslobappプロビジョニング configurationassignment の更新
description: ioslobappプロビジョニング configurationassignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9ca12e3d799c666ad7b61d9a0aa400ae2b566ca
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171394"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="31c9c-103">ioslobappプロビジョニング configurationassignment の更新</span><span class="sxs-lookup"><span data-stu-id="31c9c-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="31c9c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31c9c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31c9c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="31c9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31c9c-106">[ioslobappプロビジョニング configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="31c9c-106">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31c9c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="31c9c-107">Prerequisites</span></span>
<span data-ttu-id="31c9c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31c9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="31c9c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31c9c-110">Permission type</span></span>|<span data-ttu-id="31c9c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="31c9c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31c9c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="31c9c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31c9c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31c9c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="31c9c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31c9c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31c9c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31c9c-115">Not supported.</span></span>|
|<span data-ttu-id="31c9c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31c9c-116">Application</span></span>|<span data-ttu-id="31c9c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31c9c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31c9c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31c9c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="31c9c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31c9c-119">Request headers</span></span>
|<span data-ttu-id="31c9c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31c9c-120">Header</span></span>|<span data-ttu-id="31c9c-121">値</span><span class="sxs-lookup"><span data-stu-id="31c9c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31c9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31c9c-122">Authorization</span></span>|<span data-ttu-id="31c9c-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="31c9c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31c9c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="31c9c-124">Accept</span></span>|<span data-ttu-id="31c9c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31c9c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31c9c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="31c9c-126">Request body</span></span>
<span data-ttu-id="31c9c-127">要求本文で、 [ioslobappプロビジョニング configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="31c9c-127">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="31c9c-128">次の表に、 [ioslobappare configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="31c9c-128">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="31c9c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31c9c-129">Property</span></span>|<span data-ttu-id="31c9c-130">型</span><span class="sxs-lookup"><span data-stu-id="31c9c-130">Type</span></span>|<span data-ttu-id="31c9c-131">説明</span><span class="sxs-lookup"><span data-stu-id="31c9c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31c9c-132">id</span><span class="sxs-lookup"><span data-stu-id="31c9c-132">id</span></span>|<span data-ttu-id="31c9c-133">String</span><span class="sxs-lookup"><span data-stu-id="31c9c-133">String</span></span>|<span data-ttu-id="31c9c-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="31c9c-134">Key of the entity.</span></span>|
|<span data-ttu-id="31c9c-135">target</span><span class="sxs-lookup"><span data-stu-id="31c9c-135">target</span></span>|[<span data-ttu-id="31c9c-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="31c9c-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="31c9c-137">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="31c9c-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="31c9c-138">応答</span><span class="sxs-lookup"><span data-stu-id="31c9c-138">Response</span></span>
<span data-ttu-id="31c9c-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[ioslobappプロビジョニング configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="31c9c-139">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31c9c-140">例</span><span class="sxs-lookup"><span data-stu-id="31c9c-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="31c9c-141">要求</span><span class="sxs-lookup"><span data-stu-id="31c9c-141">Request</span></span>
<span data-ttu-id="31c9c-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="31c9c-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="31c9c-143">応答</span><span class="sxs-lookup"><span data-stu-id="31c9c-143">Response</span></span>
<span data-ttu-id="31c9c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="31c9c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




