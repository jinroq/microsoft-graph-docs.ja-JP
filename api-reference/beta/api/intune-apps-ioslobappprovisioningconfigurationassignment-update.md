---
title: IosLobAppProvisioningConfigurationAssignment を更新します。
description: IosLobAppProvisioningConfigurationAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 0212d357ceee946e8515a5143ffd7bf7307a7773
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338879"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="c8637-103">IosLobAppProvisioningConfigurationAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="c8637-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="c8637-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8637-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8637-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8637-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8637-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8637-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8637-107">[IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c8637-107">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8637-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c8637-108">Prerequisites</span></span>
<span data-ttu-id="c8637-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8637-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8637-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8637-111">Permission type</span></span>|<span data-ttu-id="c8637-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8637-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8637-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8637-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8637-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8637-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8637-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8637-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8637-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8637-116">Not supported.</span></span>|
|<span data-ttu-id="c8637-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8637-117">Application</span></span>|<span data-ttu-id="c8637-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8637-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8637-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8637-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c8637-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8637-120">Request headers</span></span>
|<span data-ttu-id="c8637-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8637-121">Header</span></span>|<span data-ttu-id="c8637-122">値</span><span class="sxs-lookup"><span data-stu-id="c8637-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8637-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8637-123">Authorization</span></span>|<span data-ttu-id="c8637-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c8637-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8637-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8637-125">Accept</span></span>|<span data-ttu-id="c8637-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8637-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8637-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8637-127">Request body</span></span>
<span data-ttu-id="c8637-128">要求の本文に[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8637-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="c8637-129">[IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="c8637-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="c8637-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8637-130">Property</span></span>|<span data-ttu-id="c8637-131">種類</span><span class="sxs-lookup"><span data-stu-id="c8637-131">Type</span></span>|<span data-ttu-id="c8637-132">説明</span><span class="sxs-lookup"><span data-stu-id="c8637-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8637-133">ID</span><span class="sxs-lookup"><span data-stu-id="c8637-133">id</span></span>|<span data-ttu-id="c8637-134">String</span><span class="sxs-lookup"><span data-stu-id="c8637-134">String</span></span>|<span data-ttu-id="c8637-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c8637-135">Key of the entity.</span></span>|
|<span data-ttu-id="c8637-136">target</span><span class="sxs-lookup"><span data-stu-id="c8637-136">target</span></span>|[<span data-ttu-id="c8637-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c8637-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c8637-138">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="c8637-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="c8637-139">応答</span><span class="sxs-lookup"><span data-stu-id="c8637-139">Response</span></span>
<span data-ttu-id="c8637-140">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c8637-140">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8637-141">例</span><span class="sxs-lookup"><span data-stu-id="c8637-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8637-142">要求</span><span class="sxs-lookup"><span data-stu-id="c8637-142">Request</span></span>
<span data-ttu-id="c8637-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8637-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="c8637-144">応答</span><span class="sxs-lookup"><span data-stu-id="c8637-144">Response</span></span>
<span data-ttu-id="c8637-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8637-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





