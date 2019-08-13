---
title: Ioslobappプロビジョニング Configurationassignment の作成
description: 新しい Ioslobappプロビジョニング Configurationassignment オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b1759df5f95b935af9704f138b839177eebc730
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330763"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="ec8bc-103">Ioslobappプロビジョニング Configurationassignment の作成</span><span class="sxs-lookup"><span data-stu-id="ec8bc-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="ec8bc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec8bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec8bc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ec8bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec8bc-106">新しい[Ioslobappプロビジョニング Configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ec8bc-106">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec8bc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ec8bc-107">Prerequisites</span></span>
<span data-ttu-id="ec8bc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec8bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec8bc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ec8bc-110">Permission type</span></span>|<span data-ttu-id="ec8bc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ec8bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec8bc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ec8bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ec8bc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec8bc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec8bc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ec8bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec8bc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec8bc-115">Not supported.</span></span>|
|<span data-ttu-id="ec8bc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ec8bc-116">Application</span></span>|<span data-ttu-id="ec8bc-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec8bc-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec8bc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ec8bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ec8bc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec8bc-119">Request headers</span></span>
|<span data-ttu-id="ec8bc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec8bc-120">Header</span></span>|<span data-ttu-id="ec8bc-121">値</span><span class="sxs-lookup"><span data-stu-id="ec8bc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec8bc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec8bc-122">Authorization</span></span>|<span data-ttu-id="ec8bc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ec8bc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec8bc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ec8bc-124">Accept</span></span>|<span data-ttu-id="ec8bc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ec8bc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec8bc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ec8bc-126">Request body</span></span>
<span data-ttu-id="ec8bc-127">要求本文で、Ioslobappプロビジョニング Configurationassignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ec8bc-127">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="ec8bc-128">次の表に、Ioslobappare Configurationassignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ec8bc-128">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="ec8bc-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec8bc-129">Property</span></span>|<span data-ttu-id="ec8bc-130">型</span><span class="sxs-lookup"><span data-stu-id="ec8bc-130">Type</span></span>|<span data-ttu-id="ec8bc-131">説明</span><span class="sxs-lookup"><span data-stu-id="ec8bc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec8bc-132">id</span><span class="sxs-lookup"><span data-stu-id="ec8bc-132">id</span></span>|<span data-ttu-id="ec8bc-133">String</span><span class="sxs-lookup"><span data-stu-id="ec8bc-133">String</span></span>|<span data-ttu-id="ec8bc-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ec8bc-134">Key of the entity.</span></span>|
|<span data-ttu-id="ec8bc-135">target</span><span class="sxs-lookup"><span data-stu-id="ec8bc-135">target</span></span>|[<span data-ttu-id="ec8bc-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ec8bc-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ec8bc-137">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="ec8bc-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="ec8bc-138">応答</span><span class="sxs-lookup"><span data-stu-id="ec8bc-138">Response</span></span>
<span data-ttu-id="ec8bc-139">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Ioslobappプロビジョニング configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ec8bc-139">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec8bc-140">例</span><span class="sxs-lookup"><span data-stu-id="ec8bc-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec8bc-141">要求</span><span class="sxs-lookup"><span data-stu-id="ec8bc-141">Request</span></span>
<span data-ttu-id="ec8bc-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ec8bc-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ec8bc-143">応答</span><span class="sxs-lookup"><span data-stu-id="ec8bc-143">Response</span></span>
<span data-ttu-id="ec8bc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ec8bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






