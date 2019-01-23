---
title: DeviceManagementScriptGroupAssignment を更新します。
description: DeviceManagementScriptGroupAssignment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bab2f5e2c363d56379e240eb6c26b95e7a0fc8b9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409980"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="53480-103">DeviceManagementScriptGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="53480-103">Update deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="53480-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="53480-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="53480-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53480-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53480-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="53480-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53480-107">[DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="53480-107">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53480-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="53480-108">Prerequisites</span></span>
<span data-ttu-id="53480-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53480-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="53480-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53480-111">Permission type</span></span>|<span data-ttu-id="53480-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="53480-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53480-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53480-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53480-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53480-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="53480-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53480-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53480-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53480-116">Not supported.</span></span>|
|<span data-ttu-id="53480-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53480-117">Application</span></span>|<span data-ttu-id="53480-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53480-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53480-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53480-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="53480-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53480-120">Request headers</span></span>
|<span data-ttu-id="53480-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53480-121">Header</span></span>|<span data-ttu-id="53480-122">値</span><span class="sxs-lookup"><span data-stu-id="53480-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53480-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53480-123">Authorization</span></span>|<span data-ttu-id="53480-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="53480-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53480-125">Accept</span><span class="sxs-lookup"><span data-stu-id="53480-125">Accept</span></span>|<span data-ttu-id="53480-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53480-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53480-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="53480-127">Request body</span></span>
<span data-ttu-id="53480-128">要求の本文に[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="53480-128">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="53480-129">[DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="53480-129">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="53480-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53480-130">Property</span></span>|<span data-ttu-id="53480-131">型</span><span class="sxs-lookup"><span data-stu-id="53480-131">Type</span></span>|<span data-ttu-id="53480-132">説明</span><span class="sxs-lookup"><span data-stu-id="53480-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53480-133">id</span><span class="sxs-lookup"><span data-stu-id="53480-133">id</span></span>|<span data-ttu-id="53480-134">String</span><span class="sxs-lookup"><span data-stu-id="53480-134">String</span></span>|<span data-ttu-id="53480-135">デバイス管理スクリプトのグループの割り当てエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="53480-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="53480-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="53480-136">targetGroupId</span></span>|<span data-ttu-id="53480-137">String</span><span class="sxs-lookup"><span data-stu-id="53480-137">String</span></span>|<span data-ttu-id="53480-138">Azure Active Directory グループの Id は、対象としてスクリプトをします。</span><span class="sxs-lookup"><span data-stu-id="53480-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="53480-139">応答</span><span class="sxs-lookup"><span data-stu-id="53480-139">Response</span></span>
<span data-ttu-id="53480-140">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="53480-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53480-141">例</span><span class="sxs-lookup"><span data-stu-id="53480-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="53480-142">要求</span><span class="sxs-lookup"><span data-stu-id="53480-142">Request</span></span>
<span data-ttu-id="53480-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53480-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="53480-144">応答</span><span class="sxs-lookup"><span data-stu-id="53480-144">Response</span></span>
<span data-ttu-id="53480-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="53480-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```




