---
title: deviceConfigurationAssignment の更新
description: deviceConfigurationAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1b3e2931e791c0d7e57e3a9e47896bf1ac7c64f5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947492"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="b11ef-103">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="b11ef-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="b11ef-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b11ef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b11ef-105">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b11ef-105">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b11ef-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b11ef-106">Prerequisites</span></span>
<span data-ttu-id="b11ef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b11ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b11ef-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b11ef-109">Permission type</span></span>|<span data-ttu-id="b11ef-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b11ef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b11ef-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b11ef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b11ef-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b11ef-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b11ef-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b11ef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b11ef-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b11ef-114">Not supported.</span></span>|
|<span data-ttu-id="b11ef-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b11ef-115">Application</span></span>|<span data-ttu-id="b11ef-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b11ef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b11ef-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b11ef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b11ef-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b11ef-118">Request headers</span></span>
|<span data-ttu-id="b11ef-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b11ef-119">Header</span></span>|<span data-ttu-id="b11ef-120">値</span><span class="sxs-lookup"><span data-stu-id="b11ef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b11ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b11ef-121">Authorization</span></span>|<span data-ttu-id="b11ef-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b11ef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b11ef-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b11ef-123">Accept</span></span>|<span data-ttu-id="b11ef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b11ef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b11ef-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b11ef-125">Request body</span></span>
<span data-ttu-id="b11ef-126">要求本文で、[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b11ef-126">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="b11ef-127">次の表に、[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b11ef-127">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="b11ef-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b11ef-128">Property</span></span>|<span data-ttu-id="b11ef-129">種類</span><span class="sxs-lookup"><span data-stu-id="b11ef-129">Type</span></span>|<span data-ttu-id="b11ef-130">説明</span><span class="sxs-lookup"><span data-stu-id="b11ef-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b11ef-131">ID</span><span class="sxs-lookup"><span data-stu-id="b11ef-131">id</span></span>|<span data-ttu-id="b11ef-132">String</span><span class="sxs-lookup"><span data-stu-id="b11ef-132">String</span></span>|<span data-ttu-id="b11ef-133">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="b11ef-133">The key of the assignment.</span></span>|
|<span data-ttu-id="b11ef-134">target</span><span class="sxs-lookup"><span data-stu-id="b11ef-134">target</span></span>|[<span data-ttu-id="b11ef-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b11ef-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b11ef-136">デバイス構成の割り当て先。</span><span class="sxs-lookup"><span data-stu-id="b11ef-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="b11ef-137">応答</span><span class="sxs-lookup"><span data-stu-id="b11ef-137">Response</span></span>
<span data-ttu-id="b11ef-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b11ef-138">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b11ef-139">例</span><span class="sxs-lookup"><span data-stu-id="b11ef-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="b11ef-140">要求</span><span class="sxs-lookup"><span data-stu-id="b11ef-140">Request</span></span>
<span data-ttu-id="b11ef-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b11ef-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b11ef-142">応答</span><span class="sxs-lookup"><span data-stu-id="b11ef-142">Response</span></span>
<span data-ttu-id="b11ef-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b11ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



