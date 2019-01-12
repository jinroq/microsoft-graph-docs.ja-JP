---
title: IosLobAppProvisioningConfigurationAssignment を作成します。
description: 新しい iosLobAppProvisioningConfigurationAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3e2138480d97047e7aa396becb24abb88feb4022
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925652"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="ec531-103">IosLobAppProvisioningConfigurationAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="ec531-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="ec531-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ec531-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec531-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec531-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec531-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ec531-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec531-107">新しい[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ec531-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ec531-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ec531-108">Prerequisites</span></span>
<span data-ttu-id="ec531-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec531-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec531-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ec531-111">Permission type</span></span>|<span data-ttu-id="ec531-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ec531-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec531-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ec531-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec531-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec531-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec531-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ec531-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec531-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec531-116">Not supported.</span></span>|
|<span data-ttu-id="ec531-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ec531-117">Application</span></span>|<span data-ttu-id="ec531-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec531-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec531-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ec531-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ec531-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec531-120">Request headers</span></span>
|<span data-ttu-id="ec531-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec531-121">Header</span></span>|<span data-ttu-id="ec531-122">値</span><span class="sxs-lookup"><span data-stu-id="ec531-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec531-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec531-123">Authorization</span></span>|<span data-ttu-id="ec531-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ec531-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec531-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ec531-125">Accept</span></span>|<span data-ttu-id="ec531-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec531-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec531-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ec531-127">Request body</span></span>
<span data-ttu-id="ec531-128">要求の本文に iosLobAppProvisioningConfigurationAssignment オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="ec531-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="ec531-129">次の表は、iosLobAppProvisioningConfigurationAssignment を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ec531-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="ec531-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec531-130">Property</span></span>|<span data-ttu-id="ec531-131">型</span><span class="sxs-lookup"><span data-stu-id="ec531-131">Type</span></span>|<span data-ttu-id="ec531-132">説明</span><span class="sxs-lookup"><span data-stu-id="ec531-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec531-133">ID</span><span class="sxs-lookup"><span data-stu-id="ec531-133">id</span></span>|<span data-ttu-id="ec531-134">String</span><span class="sxs-lookup"><span data-stu-id="ec531-134">String</span></span>|<span data-ttu-id="ec531-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ec531-135">Key of the entity.</span></span>|
|<span data-ttu-id="ec531-136">target</span><span class="sxs-lookup"><span data-stu-id="ec531-136">target</span></span>|[<span data-ttu-id="ec531-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ec531-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ec531-138">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="ec531-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="ec531-139">応答</span><span class="sxs-lookup"><span data-stu-id="ec531-139">Response</span></span>
<span data-ttu-id="ec531-140">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ec531-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec531-141">例</span><span class="sxs-lookup"><span data-stu-id="ec531-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="ec531-142">要求</span><span class="sxs-lookup"><span data-stu-id="ec531-142">Request</span></span>
<span data-ttu-id="ec531-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ec531-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ec531-144">応答</span><span class="sxs-lookup"><span data-stu-id="ec531-144">Response</span></span>
<span data-ttu-id="ec531-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ec531-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





