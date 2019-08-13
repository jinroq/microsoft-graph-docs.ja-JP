---
title: managedDeviceMobileAppConfigurationAssignment の更新
description: managedDeviceMobileAppConfigurationAssignment オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ad41617422a318354c7a547e47b3b177559d4d8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329867"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="6dead-103">managedDeviceMobileAppConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="6dead-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="6dead-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dead-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dead-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6dead-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dead-106">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6dead-106">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dead-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6dead-107">Prerequisites</span></span>
<span data-ttu-id="6dead-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6dead-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dead-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6dead-110">Permission type</span></span>|<span data-ttu-id="6dead-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6dead-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dead-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6dead-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6dead-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dead-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6dead-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6dead-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dead-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dead-115">Not supported.</span></span>|
|<span data-ttu-id="6dead-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6dead-116">Application</span></span>|<span data-ttu-id="6dead-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dead-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dead-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6dead-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6dead-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6dead-119">Request headers</span></span>
|<span data-ttu-id="6dead-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6dead-120">Header</span></span>|<span data-ttu-id="6dead-121">値</span><span class="sxs-lookup"><span data-stu-id="6dead-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dead-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dead-122">Authorization</span></span>|<span data-ttu-id="6dead-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6dead-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dead-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6dead-124">Accept</span></span>|<span data-ttu-id="6dead-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6dead-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dead-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6dead-126">Request body</span></span>
<span data-ttu-id="6dead-127">要求本文で、[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6dead-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="6dead-128">次の表に、[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6dead-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="6dead-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6dead-129">Property</span></span>|<span data-ttu-id="6dead-130">型</span><span class="sxs-lookup"><span data-stu-id="6dead-130">Type</span></span>|<span data-ttu-id="6dead-131">説明</span><span class="sxs-lookup"><span data-stu-id="6dead-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dead-132">id</span><span class="sxs-lookup"><span data-stu-id="6dead-132">id</span></span>|<span data-ttu-id="6dead-133">String</span><span class="sxs-lookup"><span data-stu-id="6dead-133">String</span></span>|<span data-ttu-id="6dead-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6dead-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="6dead-135">target</span><span class="sxs-lookup"><span data-stu-id="6dead-135">target</span></span>|[<span data-ttu-id="6dead-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6dead-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6dead-137">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="6dead-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="6dead-138">応答</span><span class="sxs-lookup"><span data-stu-id="6dead-138">Response</span></span>
<span data-ttu-id="6dead-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6dead-139">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dead-140">例</span><span class="sxs-lookup"><span data-stu-id="6dead-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dead-141">要求</span><span class="sxs-lookup"><span data-stu-id="6dead-141">Request</span></span>
<span data-ttu-id="6dead-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6dead-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="6dead-143">応答</span><span class="sxs-lookup"><span data-stu-id="6dead-143">Response</span></span>
<span data-ttu-id="6dead-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6dead-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






