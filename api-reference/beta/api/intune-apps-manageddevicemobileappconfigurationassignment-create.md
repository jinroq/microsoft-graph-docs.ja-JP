---
title: managedDeviceMobileAppConfigurationAssignment の作成
description: 新しい managedDeviceMobileAppConfigurationAssignment オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 10eeb2cdaba8b9e1c855a8e94966ceb0b95c7317
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398045"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="d1ade-103">managedDeviceMobileAppConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="d1ade-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="d1ade-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d1ade-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d1ade-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1ade-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1ade-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1ade-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1ade-107">新しい [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d1ade-107">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1ade-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d1ade-108">Prerequisites</span></span>
<span data-ttu-id="d1ade-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1ade-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d1ade-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d1ade-111">Permission type</span></span>|<span data-ttu-id="d1ade-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1ade-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1ade-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1ade-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1ade-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1ade-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d1ade-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1ade-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1ade-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1ade-116">Not supported.</span></span>|
|<span data-ttu-id="d1ade-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1ade-117">Application</span></span>|<span data-ttu-id="d1ade-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1ade-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1ade-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1ade-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d1ade-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1ade-120">Request headers</span></span>
|<span data-ttu-id="d1ade-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1ade-121">Header</span></span>|<span data-ttu-id="d1ade-122">値</span><span class="sxs-lookup"><span data-stu-id="d1ade-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1ade-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1ade-123">Authorization</span></span>|<span data-ttu-id="d1ade-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d1ade-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1ade-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d1ade-125">Accept</span></span>|<span data-ttu-id="d1ade-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1ade-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1ade-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1ade-127">Request body</span></span>
<span data-ttu-id="d1ade-128">要求本文で、managedDeviceMobileAppConfigurationAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d1ade-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="d1ade-129">次の表に、managedDeviceMobileAppConfigurationAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d1ade-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="d1ade-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1ade-130">Property</span></span>|<span data-ttu-id="d1ade-131">型</span><span class="sxs-lookup"><span data-stu-id="d1ade-131">Type</span></span>|<span data-ttu-id="d1ade-132">説明</span><span class="sxs-lookup"><span data-stu-id="d1ade-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1ade-133">id</span><span class="sxs-lookup"><span data-stu-id="d1ade-133">id</span></span>|<span data-ttu-id="d1ade-134">String</span><span class="sxs-lookup"><span data-stu-id="d1ade-134">String</span></span>|<span data-ttu-id="d1ade-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d1ade-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d1ade-136">target</span><span class="sxs-lookup"><span data-stu-id="d1ade-136">target</span></span>|[<span data-ttu-id="d1ade-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d1ade-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d1ade-138">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="d1ade-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="d1ade-139">応答</span><span class="sxs-lookup"><span data-stu-id="d1ade-139">Response</span></span>
<span data-ttu-id="d1ade-140">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d1ade-140">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1ade-141">例</span><span class="sxs-lookup"><span data-stu-id="d1ade-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1ade-142">要求</span><span class="sxs-lookup"><span data-stu-id="d1ade-142">Request</span></span>
<span data-ttu-id="d1ade-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d1ade-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d1ade-144">応答</span><span class="sxs-lookup"><span data-stu-id="d1ade-144">Response</span></span>
<span data-ttu-id="d1ade-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d1ade-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




