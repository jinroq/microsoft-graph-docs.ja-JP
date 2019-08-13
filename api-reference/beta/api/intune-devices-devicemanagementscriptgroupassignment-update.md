---
title: DeviceManagementScriptGroupAssignment の更新
description: DeviceManagementScriptGroupAssignment オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b56741024048b3f9442288970275563f1bd9142b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348880"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="58d0e-103">DeviceManagementScriptGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="58d0e-103">Update deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="58d0e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58d0e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58d0e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="58d0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58d0e-106">[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="58d0e-106">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58d0e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="58d0e-107">Prerequisites</span></span>
<span data-ttu-id="58d0e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58d0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58d0e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58d0e-110">Permission type</span></span>|<span data-ttu-id="58d0e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="58d0e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58d0e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58d0e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58d0e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58d0e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="58d0e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58d0e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58d0e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58d0e-115">Not supported.</span></span>|
|<span data-ttu-id="58d0e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58d0e-116">Application</span></span>|<span data-ttu-id="58d0e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58d0e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58d0e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58d0e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="58d0e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58d0e-119">Request headers</span></span>
|<span data-ttu-id="58d0e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58d0e-120">Header</span></span>|<span data-ttu-id="58d0e-121">値</span><span class="sxs-lookup"><span data-stu-id="58d0e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58d0e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58d0e-122">Authorization</span></span>|<span data-ttu-id="58d0e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="58d0e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58d0e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="58d0e-124">Accept</span></span>|<span data-ttu-id="58d0e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58d0e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58d0e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="58d0e-126">Request body</span></span>
<span data-ttu-id="58d0e-127">要求本文で、 [Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="58d0e-127">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="58d0e-128">次の表に、 [Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="58d0e-128">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="58d0e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58d0e-129">Property</span></span>|<span data-ttu-id="58d0e-130">型</span><span class="sxs-lookup"><span data-stu-id="58d0e-130">Type</span></span>|<span data-ttu-id="58d0e-131">説明</span><span class="sxs-lookup"><span data-stu-id="58d0e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58d0e-132">id</span><span class="sxs-lookup"><span data-stu-id="58d0e-132">id</span></span>|<span data-ttu-id="58d0e-133">String</span><span class="sxs-lookup"><span data-stu-id="58d0e-133">String</span></span>|<span data-ttu-id="58d0e-134">[デバイス管理スクリプト] グループ割り当てエンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="58d0e-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="58d0e-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="58d0e-135">targetGroupId</span></span>|<span data-ttu-id="58d0e-136">String</span><span class="sxs-lookup"><span data-stu-id="58d0e-136">String</span></span>|<span data-ttu-id="58d0e-137">スクリプトを対象としている Azure Active Directory グループの Id。</span><span class="sxs-lookup"><span data-stu-id="58d0e-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="58d0e-138">応答</span><span class="sxs-lookup"><span data-stu-id="58d0e-138">Response</span></span>
<span data-ttu-id="58d0e-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="58d0e-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58d0e-140">例</span><span class="sxs-lookup"><span data-stu-id="58d0e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="58d0e-141">要求</span><span class="sxs-lookup"><span data-stu-id="58d0e-141">Request</span></span>
<span data-ttu-id="58d0e-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="58d0e-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="58d0e-143">応答</span><span class="sxs-lookup"><span data-stu-id="58d0e-143">Response</span></span>
<span data-ttu-id="58d0e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="58d0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






