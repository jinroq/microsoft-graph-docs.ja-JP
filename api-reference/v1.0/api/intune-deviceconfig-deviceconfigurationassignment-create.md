---
title: deviceConfigurationAssignment の作成
description: 新しい deviceConfigurationAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f16992e3052f9f7017e3177bbfdf2539fe0cfd0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017638"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="a4738-103">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="a4738-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="a4738-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4738-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4738-105">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a4738-105">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4738-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a4738-106">Prerequisites</span></span>
<span data-ttu-id="a4738-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4738-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4738-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a4738-109">Permission type</span></span>|<span data-ttu-id="a4738-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a4738-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4738-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a4738-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4738-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4738-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4738-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4738-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4738-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4738-114">Not supported.</span></span>|
|<span data-ttu-id="a4738-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a4738-115">Application</span></span>|<span data-ttu-id="a4738-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4738-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4738-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a4738-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a4738-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4738-118">Request headers</span></span>
|<span data-ttu-id="a4738-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4738-119">Header</span></span>|<span data-ttu-id="a4738-120">値</span><span class="sxs-lookup"><span data-stu-id="a4738-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4738-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4738-121">Authorization</span></span>|<span data-ttu-id="a4738-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4738-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4738-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a4738-123">Accept</span></span>|<span data-ttu-id="a4738-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a4738-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4738-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a4738-125">Request body</span></span>
<span data-ttu-id="a4738-126">要求本文で、deviceConfigurationAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4738-126">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="a4738-127">次の表に、deviceConfigurationAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a4738-127">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="a4738-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4738-128">Property</span></span>|<span data-ttu-id="a4738-129">型</span><span class="sxs-lookup"><span data-stu-id="a4738-129">Type</span></span>|<span data-ttu-id="a4738-130">説明</span><span class="sxs-lookup"><span data-stu-id="a4738-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4738-131">id</span><span class="sxs-lookup"><span data-stu-id="a4738-131">id</span></span>|<span data-ttu-id="a4738-132">String</span><span class="sxs-lookup"><span data-stu-id="a4738-132">String</span></span>|<span data-ttu-id="a4738-133">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="a4738-133">The key of the assignment.</span></span>|
|<span data-ttu-id="a4738-134">target</span><span class="sxs-lookup"><span data-stu-id="a4738-134">target</span></span>|[<span data-ttu-id="a4738-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a4738-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a4738-136">デバイス構成の割り当て先。</span><span class="sxs-lookup"><span data-stu-id="a4738-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="a4738-137">応答</span><span class="sxs-lookup"><span data-stu-id="a4738-137">Response</span></span>
<span data-ttu-id="a4738-138">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a4738-138">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4738-139">例</span><span class="sxs-lookup"><span data-stu-id="a4738-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4738-140">要求</span><span class="sxs-lookup"><span data-stu-id="a4738-140">Request</span></span>
<span data-ttu-id="a4738-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a4738-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="a4738-142">応答</span><span class="sxs-lookup"><span data-stu-id="a4738-142">Response</span></span>
<span data-ttu-id="a4738-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a4738-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



