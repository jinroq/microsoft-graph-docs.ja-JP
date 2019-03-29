---
title: deviceManagementScriptAssignment を作成する
description: 新しい deviceManagementScriptAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11147c2b273da300d5c9f9123b8dde7e49d8d2cc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975407"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="6ce6f-103">deviceManagementScriptAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="6ce6f-103">Create deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="6ce6f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ce6f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ce6f-106">新しい[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-106">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ce6f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6ce6f-107">Prerequisites</span></span>
<span data-ttu-id="6ce6f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ce6f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6ce6f-110">Permission type</span></span>|<span data-ttu-id="6ce6f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6ce6f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ce6f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6ce6f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ce6f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ce6f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6ce6f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ce6f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ce6f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-115">Not supported.</span></span>|
|<span data-ttu-id="6ce6f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6ce6f-116">Application</span></span>|<span data-ttu-id="6ce6f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ce6f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6ce6f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6ce6f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ce6f-119">Request headers</span></span>
|<span data-ttu-id="6ce6f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ce6f-120">Header</span></span>|<span data-ttu-id="6ce6f-121">値</span><span class="sxs-lookup"><span data-stu-id="6ce6f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ce6f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ce6f-122">Authorization</span></span>|<span data-ttu-id="6ce6f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ce6f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6ce6f-124">Accept</span></span>|<span data-ttu-id="6ce6f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6ce6f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ce6f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6ce6f-126">Request body</span></span>
<span data-ttu-id="6ce6f-127">要求本文で、deviceManagementScriptAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-127">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="6ce6f-128">次の表に、deviceManagementScriptAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-128">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="6ce6f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ce6f-129">Property</span></span>|<span data-ttu-id="6ce6f-130">型</span><span class="sxs-lookup"><span data-stu-id="6ce6f-130">Type</span></span>|<span data-ttu-id="6ce6f-131">説明</span><span class="sxs-lookup"><span data-stu-id="6ce6f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ce6f-132">id</span><span class="sxs-lookup"><span data-stu-id="6ce6f-132">id</span></span>|<span data-ttu-id="6ce6f-133">String</span><span class="sxs-lookup"><span data-stu-id="6ce6f-133">String</span></span>|<span data-ttu-id="6ce6f-134">[デバイス管理スクリプト] グループ割り当てエンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="6ce6f-135">target</span><span class="sxs-lookup"><span data-stu-id="6ce6f-135">target</span></span>|[<span data-ttu-id="6ce6f-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6ce6f-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6ce6f-137">スクリプトを対象としている Azure Active Directory グループの Id。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="6ce6f-138">応答</span><span class="sxs-lookup"><span data-stu-id="6ce6f-138">Response</span></span>
<span data-ttu-id="6ce6f-139">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-139">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ce6f-140">例</span><span class="sxs-lookup"><span data-stu-id="6ce6f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ce6f-141">要求</span><span class="sxs-lookup"><span data-stu-id="6ce6f-141">Request</span></span>
<span data-ttu-id="6ce6f-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="6ce6f-143">応答</span><span class="sxs-lookup"><span data-stu-id="6ce6f-143">Response</span></span>
<span data-ttu-id="6ce6f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6ce6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




