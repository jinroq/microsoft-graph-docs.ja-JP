---
title: managedDeviceMobileAppConfigurationAssignment の作成
description: 新しい managedDeviceMobileAppConfigurationAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f8fb7741aeabbf941142143f03c16217dfb58b8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014075"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="2d72c-103">managedDeviceMobileAppConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="2d72c-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="2d72c-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d72c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d72c-105">新しい [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2d72c-105">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d72c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="2d72c-106">Prerequisites</span></span>
<span data-ttu-id="2d72c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d72c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d72c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2d72c-109">Permission type</span></span>|<span data-ttu-id="2d72c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2d72c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d72c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2d72c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2d72c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d72c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2d72c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2d72c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d72c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d72c-114">Not supported.</span></span>|
|<span data-ttu-id="2d72c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2d72c-115">Application</span></span>|<span data-ttu-id="2d72c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d72c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d72c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2d72c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2d72c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d72c-118">Request headers</span></span>
|<span data-ttu-id="2d72c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d72c-119">Header</span></span>|<span data-ttu-id="2d72c-120">値</span><span class="sxs-lookup"><span data-stu-id="2d72c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d72c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d72c-121">Authorization</span></span>|<span data-ttu-id="2d72c-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d72c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d72c-123">承諾</span><span class="sxs-lookup"><span data-stu-id="2d72c-123">Accept</span></span>|<span data-ttu-id="2d72c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2d72c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d72c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2d72c-125">Request body</span></span>
<span data-ttu-id="2d72c-126">要求本文で、managedDeviceMobileAppConfigurationAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2d72c-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="2d72c-127">次の表に、managedDeviceMobileAppConfigurationAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2d72c-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="2d72c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d72c-128">Property</span></span>|<span data-ttu-id="2d72c-129">型</span><span class="sxs-lookup"><span data-stu-id="2d72c-129">Type</span></span>|<span data-ttu-id="2d72c-130">説明</span><span class="sxs-lookup"><span data-stu-id="2d72c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d72c-131">id</span><span class="sxs-lookup"><span data-stu-id="2d72c-131">id</span></span>|<span data-ttu-id="2d72c-132">String</span><span class="sxs-lookup"><span data-stu-id="2d72c-132">String</span></span>|<span data-ttu-id="2d72c-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="2d72c-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="2d72c-134">target</span><span class="sxs-lookup"><span data-stu-id="2d72c-134">target</span></span>|[<span data-ttu-id="2d72c-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2d72c-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2d72c-136">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="2d72c-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="2d72c-137">応答</span><span class="sxs-lookup"><span data-stu-id="2d72c-137">Response</span></span>
<span data-ttu-id="2d72c-138">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2d72c-138">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d72c-139">例</span><span class="sxs-lookup"><span data-stu-id="2d72c-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d72c-140">要求</span><span class="sxs-lookup"><span data-stu-id="2d72c-140">Request</span></span>
<span data-ttu-id="2d72c-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2d72c-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2d72c-142">応答</span><span class="sxs-lookup"><span data-stu-id="2d72c-142">Response</span></span>
<span data-ttu-id="2d72c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2d72c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



