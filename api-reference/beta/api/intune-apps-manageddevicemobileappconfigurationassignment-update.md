---
title: managedDeviceMobileAppConfigurationAssignment の更新
description: managedDeviceMobileAppConfigurationAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ec20c87f64a61da24188977715da1f0738b1b0f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887685"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="ab8c2-103">managedDeviceMobileAppConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="ab8c2-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="ab8c2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab8c2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab8c2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab8c2-107">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-107">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab8c2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ab8c2-108">Prerequisites</span></span>
<span data-ttu-id="ab8c2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab8c2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ab8c2-111">Permission type</span></span>|<span data-ttu-id="ab8c2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ab8c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab8c2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ab8c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab8c2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab8c2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ab8c2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ab8c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab8c2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-116">Not supported.</span></span>|
|<span data-ttu-id="ab8c2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ab8c2-117">Application</span></span>|<span data-ttu-id="ab8c2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab8c2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ab8c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ab8c2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab8c2-120">Request headers</span></span>
|<span data-ttu-id="ab8c2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab8c2-121">Header</span></span>|<span data-ttu-id="ab8c2-122">値</span><span class="sxs-lookup"><span data-stu-id="ab8c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab8c2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab8c2-123">Authorization</span></span>|<span data-ttu-id="ab8c2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab8c2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab8c2-125">Accept</span></span>|<span data-ttu-id="ab8c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab8c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab8c2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ab8c2-127">Request body</span></span>
<span data-ttu-id="ab8c2-128">要求本文で、[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="ab8c2-129">次の表に、[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="ab8c2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab8c2-130">Property</span></span>|<span data-ttu-id="ab8c2-131">種類</span><span class="sxs-lookup"><span data-stu-id="ab8c2-131">Type</span></span>|<span data-ttu-id="ab8c2-132">説明</span><span class="sxs-lookup"><span data-stu-id="ab8c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab8c2-133">ID</span><span class="sxs-lookup"><span data-stu-id="ab8c2-133">id</span></span>|<span data-ttu-id="ab8c2-134">String</span><span class="sxs-lookup"><span data-stu-id="ab8c2-134">String</span></span>|<span data-ttu-id="ab8c2-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ab8c2-136">target</span><span class="sxs-lookup"><span data-stu-id="ab8c2-136">target</span></span>|[<span data-ttu-id="ab8c2-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ab8c2-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ab8c2-138">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="ab8c2-139">応答</span><span class="sxs-lookup"><span data-stu-id="ab8c2-139">Response</span></span>
<span data-ttu-id="ab8c2-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-140">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab8c2-141">例</span><span class="sxs-lookup"><span data-stu-id="ab8c2-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab8c2-142">要求</span><span class="sxs-lookup"><span data-stu-id="ab8c2-142">Request</span></span>
<span data-ttu-id="ab8c2-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ab8c2-144">応答</span><span class="sxs-lookup"><span data-stu-id="ab8c2-144">Response</span></span>
<span data-ttu-id="ab8c2-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ab8c2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





