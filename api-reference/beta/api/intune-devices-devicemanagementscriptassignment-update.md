---
title: DeviceManagementScriptAssignment を更新します。
description: DeviceManagementScriptAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 552dffca7adf6825a77e4edb65cf0ceef8fcaa83
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921585"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="57fdb-103">DeviceManagementScriptAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="57fdb-103">Update deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="57fdb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="57fdb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57fdb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57fdb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57fdb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="57fdb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57fdb-107">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="57fdb-107">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57fdb-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="57fdb-108">Prerequisites</span></span>
<span data-ttu-id="57fdb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57fdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57fdb-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="57fdb-111">Permission type</span></span>|<span data-ttu-id="57fdb-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="57fdb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57fdb-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="57fdb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57fdb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57fdb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="57fdb-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="57fdb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57fdb-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57fdb-116">Not supported.</span></span>|
|<span data-ttu-id="57fdb-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="57fdb-117">Application</span></span>|<span data-ttu-id="57fdb-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57fdb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57fdb-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="57fdb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="57fdb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57fdb-120">Request headers</span></span>
|<span data-ttu-id="57fdb-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57fdb-121">Header</span></span>|<span data-ttu-id="57fdb-122">値</span><span class="sxs-lookup"><span data-stu-id="57fdb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57fdb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="57fdb-123">Authorization</span></span>|<span data-ttu-id="57fdb-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="57fdb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57fdb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="57fdb-125">Accept</span></span>|<span data-ttu-id="57fdb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57fdb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57fdb-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="57fdb-127">Request body</span></span>
<span data-ttu-id="57fdb-128">要求の本文に[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="57fdb-128">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="57fdb-129">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="57fdb-129">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="57fdb-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57fdb-130">Property</span></span>|<span data-ttu-id="57fdb-131">型</span><span class="sxs-lookup"><span data-stu-id="57fdb-131">Type</span></span>|<span data-ttu-id="57fdb-132">説明</span><span class="sxs-lookup"><span data-stu-id="57fdb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57fdb-133">ID</span><span class="sxs-lookup"><span data-stu-id="57fdb-133">id</span></span>|<span data-ttu-id="57fdb-134">String</span><span class="sxs-lookup"><span data-stu-id="57fdb-134">String</span></span>|<span data-ttu-id="57fdb-135">デバイス管理スクリプトのグループの割り当てエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="57fdb-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="57fdb-136">ターゲット</span><span class="sxs-lookup"><span data-stu-id="57fdb-136">target</span></span>|[<span data-ttu-id="57fdb-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="57fdb-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="57fdb-138">Azure Active Directory グループの Id は、対象としてスクリプトをします。</span><span class="sxs-lookup"><span data-stu-id="57fdb-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="57fdb-139">応答</span><span class="sxs-lookup"><span data-stu-id="57fdb-139">Response</span></span>
<span data-ttu-id="57fdb-140">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="57fdb-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57fdb-141">例</span><span class="sxs-lookup"><span data-stu-id="57fdb-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="57fdb-142">要求</span><span class="sxs-lookup"><span data-stu-id="57fdb-142">Request</span></span>
<span data-ttu-id="57fdb-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="57fdb-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="57fdb-144">応答</span><span class="sxs-lookup"><span data-stu-id="57fdb-144">Response</span></span>
<span data-ttu-id="57fdb-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="57fdb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





