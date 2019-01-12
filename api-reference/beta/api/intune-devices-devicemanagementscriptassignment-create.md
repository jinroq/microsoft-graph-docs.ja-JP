---
title: DeviceManagementScriptAssignment を作成します。
description: 新しい deviceManagementScriptAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fb9f475c8aec7dabfe44c7b47cbb9ed087a31544
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974225"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="094fd-103">DeviceManagementScriptAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="094fd-103">Create deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="094fd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="094fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="094fd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="094fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="094fd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="094fd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="094fd-107">新しい[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="094fd-107">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="094fd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="094fd-108">Prerequisites</span></span>
<span data-ttu-id="094fd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="094fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="094fd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="094fd-111">Permission type</span></span>|<span data-ttu-id="094fd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="094fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="094fd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="094fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="094fd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="094fd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="094fd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="094fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="094fd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="094fd-116">Not supported.</span></span>|
|<span data-ttu-id="094fd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="094fd-117">Application</span></span>|<span data-ttu-id="094fd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="094fd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="094fd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="094fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="094fd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="094fd-120">Request headers</span></span>
|<span data-ttu-id="094fd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="094fd-121">Header</span></span>|<span data-ttu-id="094fd-122">値</span><span class="sxs-lookup"><span data-stu-id="094fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="094fd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="094fd-123">Authorization</span></span>|<span data-ttu-id="094fd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="094fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="094fd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="094fd-125">Accept</span></span>|<span data-ttu-id="094fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="094fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="094fd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="094fd-127">Request body</span></span>
<span data-ttu-id="094fd-128">要求の本文に deviceManagementScriptAssignment オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="094fd-128">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="094fd-129">次の表は、deviceManagementScriptAssignment を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="094fd-129">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="094fd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="094fd-130">Property</span></span>|<span data-ttu-id="094fd-131">種類</span><span class="sxs-lookup"><span data-stu-id="094fd-131">Type</span></span>|<span data-ttu-id="094fd-132">説明</span><span class="sxs-lookup"><span data-stu-id="094fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="094fd-133">ID</span><span class="sxs-lookup"><span data-stu-id="094fd-133">id</span></span>|<span data-ttu-id="094fd-134">String</span><span class="sxs-lookup"><span data-stu-id="094fd-134">String</span></span>|<span data-ttu-id="094fd-135">デバイス管理スクリプトのグループの割り当てエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="094fd-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="094fd-136">ターゲット</span><span class="sxs-lookup"><span data-stu-id="094fd-136">target</span></span>|[<span data-ttu-id="094fd-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="094fd-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="094fd-138">Azure Active Directory グループの Id は、対象としてスクリプトをします。</span><span class="sxs-lookup"><span data-stu-id="094fd-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="094fd-139">応答</span><span class="sxs-lookup"><span data-stu-id="094fd-139">Response</span></span>
<span data-ttu-id="094fd-140">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="094fd-140">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="094fd-141">例</span><span class="sxs-lookup"><span data-stu-id="094fd-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="094fd-142">要求</span><span class="sxs-lookup"><span data-stu-id="094fd-142">Request</span></span>
<span data-ttu-id="094fd-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="094fd-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="094fd-144">応答</span><span class="sxs-lookup"><span data-stu-id="094fd-144">Response</span></span>
<span data-ttu-id="094fd-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="094fd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





