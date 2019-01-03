---
title: assign アクション
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 0264f5aff78058887e6f219d08812eb6857737ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308177"
---
# <a name="assign-action"></a><span data-ttu-id="a9958-103">assign アクション</span><span class="sxs-lookup"><span data-stu-id="a9958-103">assign action</span></span>

> <span data-ttu-id="a9958-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a9958-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9958-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9958-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9958-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9958-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9958-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a9958-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9958-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a9958-108">Prerequisites</span></span>
<span data-ttu-id="a9958-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9958-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9958-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9958-111">Permission type</span></span>|<span data-ttu-id="a9958-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a9958-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9958-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9958-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9958-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9958-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a9958-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9958-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9958-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9958-116">Not supported.</span></span>|
|<span data-ttu-id="a9958-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9958-117">Application</span></span>|<span data-ttu-id="a9958-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9958-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9958-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9958-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="a9958-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9958-120">Request headers</span></span>
|<span data-ttu-id="a9958-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9958-121">Header</span></span>|<span data-ttu-id="a9958-122">値</span><span class="sxs-lookup"><span data-stu-id="a9958-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9958-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9958-123">Authorization</span></span>|<span data-ttu-id="a9958-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a9958-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9958-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9958-125">Accept</span></span>|<span data-ttu-id="a9958-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9958-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9958-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9958-127">Request body</span></span>
<span data-ttu-id="a9958-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9958-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a9958-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="a9958-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a9958-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9958-130">Property</span></span>|<span data-ttu-id="a9958-131">種類</span><span class="sxs-lookup"><span data-stu-id="a9958-131">Type</span></span>|<span data-ttu-id="a9958-132">説明</span><span class="sxs-lookup"><span data-stu-id="a9958-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9958-133">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="a9958-133">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="a9958-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a9958-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="a9958-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a9958-135">Not yet documented</span></span>|
|<span data-ttu-id="a9958-136">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="a9958-136">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="a9958-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a9958-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="a9958-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a9958-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a9958-139">応答</span><span class="sxs-lookup"><span data-stu-id="a9958-139">Response</span></span>
<span data-ttu-id="a9958-140">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a9958-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a9958-141">例</span><span class="sxs-lookup"><span data-stu-id="a9958-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9958-142">要求</span><span class="sxs-lookup"><span data-stu-id="a9958-142">Request</span></span>
<span data-ttu-id="a9958-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a9958-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign

Content-type: application/json
Content-length: 550

{
  "deviceManagementScriptGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
      "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
      "targetGroupId": "Target Group Id value"
    }
  ],
  "deviceManagementScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
      "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a9958-144">応答</span><span class="sxs-lookup"><span data-stu-id="a9958-144">Response</span></span>
<span data-ttu-id="a9958-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a9958-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




