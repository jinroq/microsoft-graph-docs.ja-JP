---
title: assign アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 189e7c73220ed88735ada7052367db589ad2905e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171331"
---
# <a name="assign-action"></a><span data-ttu-id="a8ae9-103">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="a8ae9-103">assign action</span></span>

> <span data-ttu-id="a8ae9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8ae9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8ae9-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a8ae9-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8ae9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a8ae9-107">Prerequisites</span></span>
<span data-ttu-id="a8ae9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a8ae9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a8ae9-110">Permission type</span></span>|<span data-ttu-id="a8ae9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a8ae9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8ae9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a8ae9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8ae9-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8ae9-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a8ae9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a8ae9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8ae9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-115">Not supported.</span></span>|
|<span data-ttu-id="a8ae9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a8ae9-116">Application</span></span>|<span data-ttu-id="a8ae9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8ae9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a8ae9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="a8ae9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8ae9-119">Request headers</span></span>
|<span data-ttu-id="a8ae9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8ae9-120">Header</span></span>|<span data-ttu-id="a8ae9-121">値</span><span class="sxs-lookup"><span data-stu-id="a8ae9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8ae9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8ae9-122">Authorization</span></span>|<span data-ttu-id="a8ae9-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8ae9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a8ae9-124">Accept</span></span>|<span data-ttu-id="a8ae9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a8ae9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8ae9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a8ae9-126">Request body</span></span>
<span data-ttu-id="a8ae9-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a8ae9-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a8ae9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8ae9-129">Property</span></span>|<span data-ttu-id="a8ae9-130">型</span><span class="sxs-lookup"><span data-stu-id="a8ae9-130">Type</span></span>|<span data-ttu-id="a8ae9-131">説明</span><span class="sxs-lookup"><span data-stu-id="a8ae9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8ae9-132">devicemanagementscriptgroupassignments</span><span class="sxs-lookup"><span data-stu-id="a8ae9-132">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="a8ae9-133">[devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a8ae9-133">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="a8ae9-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a8ae9-134">Not yet documented</span></span>|
|<span data-ttu-id="a8ae9-135">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="a8ae9-135">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="a8ae9-136">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a8ae9-136">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="a8ae9-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a8ae9-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a8ae9-138">応答</span><span class="sxs-lookup"><span data-stu-id="a8ae9-138">Response</span></span>
<span data-ttu-id="a8ae9-139">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a8ae9-140">例</span><span class="sxs-lookup"><span data-stu-id="a8ae9-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8ae9-141">要求</span><span class="sxs-lookup"><span data-stu-id="a8ae9-141">Request</span></span>
<span data-ttu-id="a8ae9-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8ae9-143">応答</span><span class="sxs-lookup"><span data-stu-id="a8ae9-143">Response</span></span>
<span data-ttu-id="a8ae9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




