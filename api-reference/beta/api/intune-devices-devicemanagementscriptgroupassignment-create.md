---
title: DeviceManagementScriptGroupAssignment を作成します。
description: 新しい deviceManagementScriptGroupAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 080db816339d544681a8cb6de87ebcc9b7e60b71
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881537"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="676fa-103">DeviceManagementScriptGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="676fa-103">Create deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="676fa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="676fa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="676fa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="676fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="676fa-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="676fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="676fa-107">新しい[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="676fa-107">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="676fa-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="676fa-108">Prerequisites</span></span>
<span data-ttu-id="676fa-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="676fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="676fa-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="676fa-111">Permission type</span></span>|<span data-ttu-id="676fa-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="676fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="676fa-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="676fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="676fa-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="676fa-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="676fa-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="676fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="676fa-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="676fa-116">Not supported.</span></span>|
|<span data-ttu-id="676fa-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="676fa-117">Application</span></span>|<span data-ttu-id="676fa-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="676fa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="676fa-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="676fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="676fa-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="676fa-120">Request headers</span></span>
|<span data-ttu-id="676fa-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="676fa-121">Header</span></span>|<span data-ttu-id="676fa-122">値</span><span class="sxs-lookup"><span data-stu-id="676fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="676fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="676fa-123">Authorization</span></span>|<span data-ttu-id="676fa-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="676fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="676fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="676fa-125">Accept</span></span>|<span data-ttu-id="676fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="676fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="676fa-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="676fa-127">Request body</span></span>
<span data-ttu-id="676fa-128">要求の本文に deviceManagementScriptGroupAssignment オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="676fa-128">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="676fa-129">次の表は、deviceManagementScriptGroupAssignment を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="676fa-129">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="676fa-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="676fa-130">Property</span></span>|<span data-ttu-id="676fa-131">種類</span><span class="sxs-lookup"><span data-stu-id="676fa-131">Type</span></span>|<span data-ttu-id="676fa-132">説明</span><span class="sxs-lookup"><span data-stu-id="676fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="676fa-133">ID</span><span class="sxs-lookup"><span data-stu-id="676fa-133">id</span></span>|<span data-ttu-id="676fa-134">String</span><span class="sxs-lookup"><span data-stu-id="676fa-134">String</span></span>|<span data-ttu-id="676fa-135">デバイス管理スクリプトのグループの割り当てエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="676fa-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="676fa-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="676fa-136">targetGroupId</span></span>|<span data-ttu-id="676fa-137">String</span><span class="sxs-lookup"><span data-stu-id="676fa-137">String</span></span>|<span data-ttu-id="676fa-138">Azure Active Directory グループの Id は、対象としてスクリプトをします。</span><span class="sxs-lookup"><span data-stu-id="676fa-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="676fa-139">応答</span><span class="sxs-lookup"><span data-stu-id="676fa-139">Response</span></span>
<span data-ttu-id="676fa-140">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="676fa-140">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="676fa-141">例</span><span class="sxs-lookup"><span data-stu-id="676fa-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="676fa-142">要求</span><span class="sxs-lookup"><span data-stu-id="676fa-142">Request</span></span>
<span data-ttu-id="676fa-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="676fa-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="676fa-144">応答</span><span class="sxs-lookup"><span data-stu-id="676fa-144">Response</span></span>
<span data-ttu-id="676fa-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="676fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```





