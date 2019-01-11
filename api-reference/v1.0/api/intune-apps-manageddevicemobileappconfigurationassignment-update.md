---
title: managedDeviceMobileAppConfigurationAssignment の更新
description: managedDeviceMobileAppConfigurationAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 58d28cb3e80f127f164e65861a15c230ef2d45fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864233"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="81a6f-103">managedDeviceMobileAppConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="81a6f-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="81a6f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="81a6f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81a6f-105">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="81a6f-105">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="81a6f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="81a6f-106">Prerequisites</span></span>
<span data-ttu-id="81a6f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81a6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81a6f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81a6f-109">Permission type</span></span>|<span data-ttu-id="81a6f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="81a6f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81a6f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81a6f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81a6f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81a6f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="81a6f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81a6f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81a6f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81a6f-114">Not supported.</span></span>|
|<span data-ttu-id="81a6f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81a6f-115">Application</span></span>|<span data-ttu-id="81a6f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81a6f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81a6f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81a6f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="81a6f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81a6f-118">Request headers</span></span>
|<span data-ttu-id="81a6f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81a6f-119">Header</span></span>|<span data-ttu-id="81a6f-120">値</span><span class="sxs-lookup"><span data-stu-id="81a6f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81a6f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="81a6f-121">Authorization</span></span>|<span data-ttu-id="81a6f-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="81a6f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81a6f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="81a6f-123">Accept</span></span>|<span data-ttu-id="81a6f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="81a6f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81a6f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="81a6f-125">Request body</span></span>
<span data-ttu-id="81a6f-126">要求本文で、[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="81a6f-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="81a6f-127">次の表に、[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="81a6f-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="81a6f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81a6f-128">Property</span></span>|<span data-ttu-id="81a6f-129">種類</span><span class="sxs-lookup"><span data-stu-id="81a6f-129">Type</span></span>|<span data-ttu-id="81a6f-130">説明</span><span class="sxs-lookup"><span data-stu-id="81a6f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81a6f-131">ID</span><span class="sxs-lookup"><span data-stu-id="81a6f-131">id</span></span>|<span data-ttu-id="81a6f-132">String</span><span class="sxs-lookup"><span data-stu-id="81a6f-132">String</span></span>|<span data-ttu-id="81a6f-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="81a6f-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="81a6f-134">target</span><span class="sxs-lookup"><span data-stu-id="81a6f-134">target</span></span>|[<span data-ttu-id="81a6f-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="81a6f-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="81a6f-136">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="81a6f-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="81a6f-137">応答</span><span class="sxs-lookup"><span data-stu-id="81a6f-137">Response</span></span>
<span data-ttu-id="81a6f-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="81a6f-138">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81a6f-139">例</span><span class="sxs-lookup"><span data-stu-id="81a6f-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="81a6f-140">要求</span><span class="sxs-lookup"><span data-stu-id="81a6f-140">Request</span></span>
<span data-ttu-id="81a6f-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81a6f-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="81a6f-142">応答</span><span class="sxs-lookup"><span data-stu-id="81a6f-142">Response</span></span>
<span data-ttu-id="81a6f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="81a6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



