---
title: DeviceManagementScriptAssignment の更新
description: DeviceManagementScriptAssignment オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a2acc06daf52394246936b97e0a53be7b5524604
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310424"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="99a32-103">DeviceManagementScriptAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="99a32-103">Update deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="99a32-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99a32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99a32-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="99a32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99a32-106">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="99a32-106">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99a32-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="99a32-107">Prerequisites</span></span>
<span data-ttu-id="99a32-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99a32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99a32-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="99a32-110">Permission type</span></span>|<span data-ttu-id="99a32-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="99a32-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99a32-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="99a32-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99a32-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99a32-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="99a32-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="99a32-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99a32-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99a32-115">Not supported.</span></span>|
|<span data-ttu-id="99a32-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="99a32-116">Application</span></span>|<span data-ttu-id="99a32-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99a32-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99a32-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="99a32-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="99a32-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="99a32-119">Request headers</span></span>
|<span data-ttu-id="99a32-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="99a32-120">Header</span></span>|<span data-ttu-id="99a32-121">値</span><span class="sxs-lookup"><span data-stu-id="99a32-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99a32-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="99a32-122">Authorization</span></span>|<span data-ttu-id="99a32-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="99a32-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99a32-124">承諾</span><span class="sxs-lookup"><span data-stu-id="99a32-124">Accept</span></span>|<span data-ttu-id="99a32-125">application/json</span><span class="sxs-lookup"><span data-stu-id="99a32-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99a32-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="99a32-126">Request body</span></span>
<span data-ttu-id="99a32-127">要求本文で、 [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="99a32-127">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="99a32-128">次の表に、 [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="99a32-128">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="99a32-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99a32-129">Property</span></span>|<span data-ttu-id="99a32-130">型</span><span class="sxs-lookup"><span data-stu-id="99a32-130">Type</span></span>|<span data-ttu-id="99a32-131">説明</span><span class="sxs-lookup"><span data-stu-id="99a32-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99a32-132">id</span><span class="sxs-lookup"><span data-stu-id="99a32-132">id</span></span>|<span data-ttu-id="99a32-133">String</span><span class="sxs-lookup"><span data-stu-id="99a32-133">String</span></span>|<span data-ttu-id="99a32-134">[デバイス管理スクリプト] グループ割り当てエンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="99a32-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="99a32-135">target</span><span class="sxs-lookup"><span data-stu-id="99a32-135">target</span></span>|[<span data-ttu-id="99a32-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="99a32-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="99a32-137">スクリプトを対象としている Azure Active Directory グループの Id。</span><span class="sxs-lookup"><span data-stu-id="99a32-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="99a32-138">応答</span><span class="sxs-lookup"><span data-stu-id="99a32-138">Response</span></span>
<span data-ttu-id="99a32-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="99a32-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99a32-140">例</span><span class="sxs-lookup"><span data-stu-id="99a32-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="99a32-141">要求</span><span class="sxs-lookup"><span data-stu-id="99a32-141">Request</span></span>
<span data-ttu-id="99a32-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="99a32-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="99a32-143">応答</span><span class="sxs-lookup"><span data-stu-id="99a32-143">Response</span></span>
<span data-ttu-id="99a32-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="99a32-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






